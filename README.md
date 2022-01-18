# consecutive_arrayele_sum
# Enter your code here. Read input from STDIN. Print output to STDOUT
# Enter your code here. Read input from STDIN. Print output to STDOUT
def s(l,n):
    summ=0
    m=0
    for i in range(n):
        summ+=l[i]
        if(summ>m):
            m=summ
        if(summ<0):
            summ=0
    return m
            

n=int(input())
l=list(map(int,input().split()))
ans=s(l,n)
print(ans)

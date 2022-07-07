# 나머지가 1이 되는 수 찾기

def solution(n):
    answer = []
    for i in range(2, n):
        if n % i == 1:
            answer.append(i)
            break

    return min(answer)

#print(solution(100))
#ㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡㅡ

def solution(n):
    answer = 0

    for divisior in range(2, (n-1)//2 +1) : #2부터~반값까지
        if (n-1) % divisior == 0: #약수가 있다면
            answer = divisior
            break 
        else:
            answer = n-1 #약수가 없다면 본인
    return answer

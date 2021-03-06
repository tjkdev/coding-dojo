# 문제 설명
두 수를 입력받아 두 수의 최대공약수와 최소공배수를 반환하는 함수, 
solution을 완성해 보세요. 배열의 맨 앞에 최대공약수, 
그다음 최소공배수를 넣어 반환하면 됩니다. 
예를 들어 두 수 3, 12의 최대공약수는 3, 
최소공배수는 12이므로 solution(3, 12)는 [3, 12]를 반환해야 합니다.

제한 사항
두 수는 1이상 1000000이하의 자연수입니다.

입출력 예  
n	m	return  
3	12	[3, 12]  
2	5	[1, 10]  

# 해결법
1. 두 수를 입력 받는다.
2. 각 수의 공약수를 모두 구한다.  
 2-1. 1부터 시작하여 나누는 수를 계속 1씩 증가시키면서 나머지가 0인 숫자는 공약수 
 배열에 추가한다.
 2-2. 나누는 수가 공약수 배열에 포함되어 있으면 (2-1) 작업을 중지한다.
 2-3. 나누는 수와 나눈 몫이 같으면 (2-1) 작업을 중지한다.
3. 각 공약수 에서 공통된 수 중에서 가장 큰 값이 최대 공약수가 된다.
4. 최대 공약수로 각 수를 나눈 몫들을 최대 공약수와 곱하면 최소 공배수가 된다.



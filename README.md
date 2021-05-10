>>> int(a)
100
>>> int(a) + 100
200
>>> a = int(input())
400
>>> a
400
>>> a = int(input('정수 입력 : '))
정수 입력 : 500
>>> city = input('어디서 오셨나요 : ')
어디서 오셨나요 : 부산사
>>> city
'부산사'
>>> a = float(input('실수 입력 : '))
실수 입력 : 20.5478
>>> a
20.5478
>>> print(a, city)
20.5478 부산사
>>> 
>>> 
>>> print(' aa \t bb \t cc \n dd \t ee \a ff \b gg')
 aa 	 bb 	 cc 
 dd 	 ee  ff  gg
>>> print(" 서울은 좁아요 " "아주 좁아요 " '정말 좁아요')
 서울은 좁아요 아주 좁아요 정말 좁아요
>>> print(" 서울은 좁아요 \t\t " "아주 좁아요 \n" '정말 좁아요')
 서울은 좁아요 		 아주 좁아요 
정말 좁아요
>>> age = 20
>>> name = '빌 게이츠'
>>> print(name, '님은 ', age, '살')
빌 게이츠 님은  20 살
>>> 
>>> print(' %s, %d ' %(name, age))
 빌 게이츠, 20 
>>> 

>>> print(' [%d] [%10d] [%-10d] ' %(5, 5, 5))
 [5] [         5] [5         ] 
>>> 
>>> print(' {} {} '.format(10, 'seoul'))
 10 seoul 
>>> 
>>> print(' {} {} {} '.format(10, 3.14, 'seoul'))
 10 3.14 seoul 

>>> print(' {} {} {} '.format(10, 30, 'seoul'))
 10 30 seoul 
>>> print(' {0} {1} {2} '.format(10, 30, 'seoul'))
 10 30 seoul 
>>> print(' {2} {2} {2} '.format(10, 30, 'seoul'))
 seoul seoul seoul 
>>> print(' [{2}] [{2}] [{2}] '.format(10, 30, 'seoul'))
 [seoul] [seoul] [seoul] 
>>> print(' [{:20}] [{:10}] [{:20}] '.format(10, 30, 'seoul'))
 [                  10] [        30] [seoul               ] 
>>> print(' [{:<20}] [{:<10}] [{:<20}] '.format(10, 30, 'seoul'))
 [10                  ] [30        ] [seoul               ] 
>>> print(' [{:>20}] [{:>30}] [{:>20}] '.format(10, 30, 'seoul'))
 [                  10] [                            30] [               seoul] 
>>> print(' [{:>20}] [{:^30}] [{:>20}] '.format(10, 30, 'seoul'))
 [                  10] [              30              ] [               seoul] 
>>> print(' [{:>20}] [{:^30}] [{:>20}] '.format(10, 3.14, 'seoul'))
 [                  10] [             3.14             ] [               seoul] 

>>> print(' [{:>20}] [{:2f}] [{:>20}] '.format(10, 3.14, 'seoul'))
 [                  10] [3.140000] [               seoul] 
>>> print(' [{:>20}] [{:.2f}] [{:>20}] '.format(10, 3.14, 'seoul'))
 [                  10] [3.14] [               seoul] 
>>> print(' [{:>20}] [{:.10f}] [{:>20}] '.format(10, 3.14, 'seoul'))
 [                  10] [3.1400000000] [               seoul] 
>>> 
>>> print(' [{:>20}] [{:.30f}] [{:>20}] '.format(10, 3.14, 'seoul'))
 [                  10] [3.140000000000000124344978758018] [               seoul] 
>>> 
>>> print(' %f,  %.2f, %.10f'.format(2.13, 2.13, 2.13))
 %f,  %.2f, %.10f

>>> print(' {:2f},  %.2f, %.10f'.format(2.13, 2.13, 2.13))
 2.130000,  %.2f, %.10f
>>> print(' {:2f},  10f, %.10f'.format(2.13, 2.13, 2.13))
 2.130000,  10f, %.10f

>>> print(' %f,  %.2f, %.10f' % (2.13, 2.13, 2.13))
 2.130000,  2.13, 2.1300000000
>>> 
>>> 
>>> print(' %f,  %.2f, %.10f' % (2.13, 2.686854734613, 2.13))
 2.130000,  2.69, 2.1300000000
>>> 
>>> Sum = 0
>>> range(10)
range(0, 10)
>>> range(1, 11)
range(1, 11)
>>> for i in range(10):
	print(i)

	
0
1
2
3
4
5
6
7
8
9
>>> for i in range(0, 10):
	print(i, end = '\n')

	
0
1
2
3
4
5
6
7
8
9
>>> for i in range(0, 10):
	print(i, end = '\t')

	
0	1	2	3	4	5	6	7	8	9	
>>> for i in range(0, 10):
	print(i, end = '  ')

	
0  1  2  3  4  5  6  7  8  9  
>>> for i in range(1, 11):
	print(i, end = '  ')

	
1  2  3  4  5  6  7  8  9  10  
>>> for i in range(1, 100, 5):
	print(i, end = '  ')

	
1  6  11  16  21  26  31  36  41  46  51  56  61  66  71  76  81  86  91  96  
>>> for i in range(5, 100, 5):
	print(i, end = '  ')

	
5  10  15  20  25  30  35  40  45  50  55  60  65  70  75  80  85  90  95  
>>> 
>>> 
>>> 
>>> 
>>> 
>>> 
>>> Sum = 0
>>> for i in range(1, 11):
	Sum = Sum + i

	
>>> Sum
55
>>> for i in range(1, 101):
	Sum = Sum + i

	
>>> print(Sum)
5105
>>> Sum = 0
>>> for i in range(1, 101):
	Sum = Sum + i

	
>>> print(Sum)
5050
>>> for i in range(2, 101, 2):
	Sum = Sum + i

	
>>> Sum2 = 0.0
>>> for i in range(100):
	Sum = Sum + 0.1

	
>>> for i in range(100):
	Sum2 = Sum2 + 0.1

	
>>> Sum2
9.99999999999998
>>> print('[ %f ]' %(Sum2))
[ 10.000000 ]
>>> print('[ %.30f ]' %(Sum2))
[ 9.999999999999980460074766597245 ]
>>> print('[ %.3f ]' %(Sum2))
[ 10.000 ]
>>> 
>>> 
>>> 
>>> 
>>> 

>>> 


>>> a = int(input('정수 : '))
정수 : 30
>>> b = int(input('정수 : '))
정수 : 50
>>> 
>>> print(a, b, a+b)
30 50 80
>>> a, b = input().split()
30 50
>>> a, b
('30', '50')
>>> a, b = input().split()
4 6
>>> a, b = input().split()
3 	6


>>> f = open('c:\\dd\\aa.txt', 'r', encoding='utf8')
>>> print(f.read())
오늘은 화요일
비가 옵니다.
내일은 나의 날입니다.
>>> f2 = open('c:\\dd\\bb.txt', 'w', encoding='utf8')
>>> f2.write('파이썬은 짱입니다. \n')
12
>>> f2.write('위의 말은 사실입니다. \n')
14
>>> f.close()
>>> f2.close()
>>> f3 = open('c:\\dd\\bb.txt', 'a', encoding='utf8')
>>> for i in range(5):
	name = input('친구 이름 : ')
	f3.write(name)

	
친구 이름 : 이승만
3
친구 이름 : 박정희
3
친구 이름 : 전두환
3
친구 이름 : 노태우
3
친구 이름 : 김영상
3
>>> f3.close()
>>> 

import random
import string
point3=random.randrange(1,50)
def caishu():
    kaish=input('输入你猜的数字(1——50)：')
    kaishi=int(kaish)
    if kaishi==point3:
        print('double win!!')
    elif kaishi>point3:
        print('Lose...')
        caishu()
    else :
        print('win!')


def caidaxiao():
    print('<<<<<<<GAME STARTS!>>>>>>>>>')
    cho = input('Choose small or big：')
    point1 = random.randrange(1, 7)
    point = random.randrange(1, 7)
    point2 = random.randrange(1, 7)
    sum=point1+point+point2
    if cho=='big'and 11<=sum<=18:
        print('THE POINTS ARE', point, point2, point1)
        print('won')

    elif cho=='small'and 3<=sum<=10:
        print('THE POINTS ARE', point, point2, point1)
        print('won')
    else:
        print('THE POINTS ARE', point, point2, point1)
        print('you lose!!!!!!hhh')



def bet():
    begin=1000
    while begin>0:
        print('<<<<<<<GAME STARTS!>>>>>>>>>')
        muc=input('How much you wanna bet?')
        much=int(muc)
        cho = input('Choose small or big：')
        point1 = random.randrange(1, 7)
        point = random.randrange(1, 7)
        point2 = random.randrange(1, 7)
        sum = point1 + point + point2
        if cho == 'big' and 11 <= sum <= 18:
            print('THE POINTS ARE', point, point2, point1)
            begin=begin+much
            print('won', much,'now you have',begin)
        elif cho == 'small' and 3 <= sum <= 10:
            print('THE POINTS ARE', point, point2, point1)
            begin = begin + much
            print('won', much, 'now you have', begin)
        else:
            print('THE POINTS ARE', point, point2, point1)
            begin = begin - much
            print('you lose!!!!!!', much, 'now you have', begin)
    print('GAME OVER!')



def shouji():
    CN_MOBILE=[134,135,136,137,138,139]
    CN_UNIO=[130,131,132,155]
    CN_TETCOM=[133,153,180]
    GET=input('Enter your numner:')
    if int(GET)<=10000000000:
        print('should in 11')
        shouji()
    elif int(GET)<12999999999:
        print('no such a operator')
        shouji()
    else:
        if GET[:3] in CN_MOBILE:
            print('cn')
        elif GET[:3] in CN_TETCOM:
            print('tetcom')
        elif GET[:3] in CN_UNIO:
            print('union')
            print('we will send a message to your phone')
        else:
            print('...')


def number_test():
    while True:
        number=input('enter your number:')
        CN_MOBILE = [134, 135, 136, 137, 138, 139]
        CN_UNIO = [130, 131, 132, 155]
        CN_TETCOM = [133, 153, 180]
        first_three=int(number[0:3])
        if len(number)==11:
            if first_three in CN_TETCOM:
                print('cntetcom')
            elif first_three in CN_MOBILE:
                print('mobile')
            elif first_three in  CN_UNIO:
                print('unio')
                break
            else:print('no such operators')
        else:print('11')

weekday=['MONDAY','TUESDAY','WEDNESDAY','THURSDAY','FRIDAY']

all_in_list=[
    1,
    1.0,
    'a word',
    print(1),
    True,
    [1,2],
    (1,2),
    {'key':'value'}
]

weekday.insert(1,'chouzhu')
weekday[0:0]=['pig']
weekday.remove('pig')
weekday[0]='me'
del weekday[1:3]

VASDAQ_code={
    'BIDU':'BAIDU',
    'SINA':'Sina',
    'YOKU':'Youku'
}
VASDAQ_code['sg']='gaoyuan'
VASDAQ_code.update({'FB':'facebook'})
del VASDAQ_code['FB']

letters=('a','b','c','d','e','f','g')

a_set={1,2,3,4}
a_set.add(5)
a_set.discard(5)

num_list=[6,2,7,4,1,3,5]
print(sorted(num_list,reverse=True))
str=['m','sg','gy']
for c,b in zip(num_list,str):
    print(b,'is',c)


a=[]
for i in range(1,11):
    a.append(i)


b=[i.lower() for i in 'ABCDEFGHIGKLMN']


d={i:j.upper() for i,j in zip(range(1,6),'abcde')}
print(d)



letterss=['a','b','c']
for numm,letterss in enumerate(letterss):
    print(letterss,'is',numm+1)

path='/Users/Administrator/Desktop/Walden.txt'
with open(path,'r') as text:
    words=text.read().split()
    print(words)
    for word in words:
        print('{}-{}times'.format(word,words.count(word)))

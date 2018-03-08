print('Hello World!')
def f_c(C):
      f=C*9/5+32
      return str(f)+'F'
fc2=f_c(32)
print(fc2)
length=len('I can do this!!!')
print(length)
def kg_g(weight):
      kg=weight/1000.0
      return '体重为'+str(kg)+'kg'
print(kg_g(500))
def third_a(first,second):
    return 'THE THIRD SIDE IS {}'.format((first**2+second**2)**(1/2))
print(third_a(3,4))
def trapezoid_area(base_up,base_down,height=3):
    return 1/2*(base_up+base_down)*height
print(trapezoid_area(1,2,3))
print(trapezoid_area(height=3,base_down=2,base_up=1))
print('   *','  * *',' * * *','   |  ',sep='\n')
print(trapezoid_area(1,2,5))
file=open('C://Users/Administrator/Desktop/test.txt','w')
file.write('Hello World !')
def text_create(name,msg):
    desktop_path='/Users/Administrator/Desktop/'
    full_path=desktop_path+name+'.txt'
    file=open(full_path,'w')
    file.write(msg)
    file.close()
    print('Done')
text_create('hello','hello world')
def text_filter(word,censored_word='lame',changed_word='Awesome'):
    return word.replace(censored_word,changed_word)
print(text_filter('Python is lame!'))
def text_censored_create(name,msg):
    clean_msg=text_filter(msg)
    text_create(name,clean_msg)
    print('OK!')
text_censored_create('Try','lame!lame!lame!')
PYTHON初体验！！！！！！！！！

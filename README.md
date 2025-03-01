# LearnPython

-	Chạy trương trình bằng Terminal   
Vd : Py file.py

-	Lệnh output 
Print(“ hello word “)

2. Variable
x = "bro" 
last_name = "Long"
print(x) 
print(type(x)) # type dung de lay kieu du lieu cua x
print("Hello " + x) # noi hai chuoi lai voi nhau || print(x + last_name)
y = 21 
print(y)
z = True    
print(z == True) # tra ve True vi day la bien dung sai 

#----------------------------------------------------------------------------------------#
# 3 kieu du lieu ( int , double , float. long , short , boolean )
# 1. int
age = 18 
age+= 1   # ||age = age + 1
print(age)
print('Your age is: ' + str(age)) # chuyen kieu du lieu int thanh str

# 2. float : floating point number ( A decimal number) so thuc
height = 1.75
print(type(height))
print('My height : '+ str(height))

# 3. boolean : True or False tra ve ket qua dung sai
human = True 
# print(type(human))
print('Are you human? ' + str(human))

#----------------------------------------------------------------------------------------#

#4 muiltiple assignment : cho phep gan nhieu bien cung mot luc 

name , age , height = 'Long', 21, 1.75
ages = number = heights = 22 # gan 22 cho ca 3 bien 
print(name)
print(age)
print(height)
print("\n")
print(ages)
print(number)
print(heights)
#----------------------------------------------------------------------------------------#

print("\n")
#5 string method 
Ynames = "long"
print(len(Ynames)) # do dai cua chuoi
print(Ynames.find("o")) # tim kiem chuoi trong chuoi
print(Ynames.capitalize()) # viet hoa chu cai dau tien 
print(Ynames.upper()) # viet hoa tat ca chu cai 
print(Ynames.lower()) # viet thuong tat ca chu cai
print(Ynames.isdigit()) # kiem tra xem co phai la so hay khong
print(Ynames.isalpha()) # kiem tra xem co phai la chu cai hay khong
print(Ynames.count("l")) # dem so lan xuat hien cua chuoi trong chuoi
print(Ynames.replace("l","L")) # thay the chuoi trong chuoi
print(Ynames.split()) # tach chuoi thanh list
print(Ynames.strip()) # loai bo khoang trang dau va cuoi chuoi
print(Ynames.startswith("l")) # kiem tra xem chuoi co bat
print(Ynames.endswith("g")) # kiem tra xem chuoi co ket thuc bang chuoi do hay khong
print(Ynames.islower()) # kiem tra xem chuoi co viet thuong hay khong
print(Ynames.isupper()) # kiem tra xem chuoi co viet hoa hay khong
print(Ynames.istitle()) # kiem tra xem chuoi co viet hoa chu cai dau tien hay khong
print(Ynames*3) # in chuoi 3 lan



#----------------------------------------------------------------------------------------#

#6type cast : chuyen doi kieu du lieu 

a = 1 # int
b = 2.5 # float
c = "3" # string
c = int(c) # chuyen doi string thanh int

print(str(a)) # chuyen doi int thanh string
print(int(b)) # chuyen doi float thanh int
print(float(c)) # chuyen doi string thanh float 
print("\n")
print(c*3) # nhan chuoi voi so 3 vì đã chuyển đổi c sang int nên mới thành 9 chứ kh đổi thì sẽ in ra 333

 # nếu muốn in ra cùng với chuỗi phía trước thì phải chuyển c sang string 
print("this is number : " + str(c))

#----------------------------------------------------------------------------------------#

#7 user input : nhap du lieu tu ban phim

name = input(" What's your name ? ")
print("Hello " + name)
age = input("How old are you ? ") # nếu lỗi thì đây là cách : age = int(input("How old are you ? "))
print("Your age is : " + age )
height = input("How tall are you ? ")
print("Your height is : " + height)



#8 math library
import math
pi = 3.14 
x = 1 
y = 2 
z = 3
# print(round(pi)) # hàm làm tròn && round(number, ndigits)
# # các hàm trong math cơ bản 

# print(math.ceil(pi)) # làm tròn lên số nguyên gần nhất 
# print(math.floor(pi)) # làm tròn xuống số nguyên gần nhất 
# print(math.trunc(pi)) # hàm chỉ lấy số nguyên , bỏ phần thập phân 
# print(math.fabs(pi)) # hàm trả về giá trị tuyệt đối 
print("\n")
# lũy thừa và căn bậc
print(math.pow(2,3)) # hàm mũ 
print(math.sqrt(100)) # hàm căn bậc 2  dùng pi thay 100 là lỗi
print(abs(pi)) # hàm giá trị tuyệt đối 
print(max(x,y,z)) # hàm tìm số lớn nhất
print(min(x,y,z)) # hàm tìm số nhỏ nhất 
#----------------------------------------------------------------------------------------#
#9 String silcing : cắt chuỗi

name = "what's up bro??"

lastst = name[:3] # cắt từ đầu đến vị trí thứ 3
strr = name[4:8] # cắt từ vị trí thứ 4 đến vị trí thứ 8
strr1 = name[9:] # cắt từ vị trí thứ 9 đến hết chuỗi
stringg = name [0:12:2] # cắt từ vị trí thứ 0 đến vị trí thứ 8 với bước nhảy là 2 0:w 2:h 4:t 6:p 8:r ...
reversedname = name[::-1] # đảo ngược chuỗi

print(lastst)
print(strr)
print(strr1)
print(stringg)
print(reversedname)

website1 = "http://google.com"
website2 = "http://wikipedia.com"

slice = slice(7,-4) # cắt chuỗi từ vị trí thứ 7 đến vị trí thứ -4
print(website1[slice])
print(website2[slice])
#----------------------------------------------------------------------------------------#
#10 if statement 
age = int(input("How old are you ? "))

if age < 18 : 
    print("You are a child")
elif age >= 18 and age < 30 :
    print("You are young")
elif age >= 100 : 
    print("You are a century old")
else :
    print("You are old")





#11 logical  operations and or && not 

temp = int(input("What's the temperature ? "))

if not( temp >=0 and temp <= 30 ) :
    print("The weather is nice")
    print("go ouside")
elif not ( temp < 0  or temp >= 30 ) :
    print("The weather is bad")
    print("stay home")


# while loop a statement will excute it's block of code 
# as long as it's condition is true.

# while 1==1: # vòng lặp vô hạn
#     print("In the loop")

namer = "" # khi đặt namer = None thì nó sẽ không bằng rỗng

while namer == "":
    namer = input("Enter your name: ")
    print("Hello "+ namer)

#----------------------------------------------------------------------------------------#


#12 for loop : a statement that will excute it's block of code 
# a limited amount of time
# while = unlimited
# for = limited

# import time

# for i in range(10): # vòng lặp in ra từ 0 đến 9
#     print(i) # nếu cho i+1 thì sẽ in ra them 10 

# for i in range(50,100): # vòng lặp in ra từ 50 đến 99
#     print(i)
# for i in range(50,100,2): # vòng lặp in ra từ 50 đến 99 với bước nhảy là 2
#     print(i)
# for i in "Yo bro": # in ra vòng từng ký tự của chuỗi
#     print(i)

# for seconds in range(10,0,-1): # in ra từ 10 đến 1
#     print(seconds)
#     time.sleep(1) # dừng 1s   
# print("Happy New Year") 

#----------------------------------------------------------------------------------------#

#13 nested loops : a loop inside another loop
row = int(input("how many rows ? "))
columns = int(input("how many columns? "))
symbol = input("enter your symbol ? ")

for i in range(row):
    for j in range(columns):
        print(symbol, end="")
    print() # để xuống dòng
---------------------------------------------------------------
#14  loop control statements : change a loops excute from its normal sequence
# break : used to exit a loop
# continue : skips to the next iteration of the loop
# pass : does nothing, acts as a placeholder

# loop control statements : change a loops excute from its normal sequence
# break : used to exit a loop
# continue : skips to the next iteration of the loop
# pass : does nothing, acts as a placeholder
a = "123-456-789"
for i in range(10):
    if i == 5:
        break
    print(i)

    while True: 
        for i in a:
            if a == "-":
                continue
            print(i , end="")

for i in range(10,100):
    if i == 20:
        pass
    else:
        print(i)

while True:
    name = input("Enter your name: ")
    if name != "":
        break

---------------------------------------------------------------

#15 list = used to store multiple items in a single variable

food = ["pizza", "hamburger", "hotdog", "spaghetti", "pudding"]
#print(food) # in ra toàn bộ list
# food[0] = "sushi" # thay đổi phần tử trong list
# print(food[0]) # in ra từ sushi vì food[0] đã được gán chính xác sushi

food.append(" ice cream ") # thêm phần tử vào cuối list
food.remove("hamburger")# xóa phần tử hambuyrger trong list
food.pop() # xóa phần tử cuối cùng trong list
food.sort() # sắp xếp list theo thứ tự abc
# food.clear() # xóa toàn bộ list
print(food)

for x in food:
    print(x) # in ra từng phần tử trong list bằng hàng dọc
---------------------------------------------------------------
#16 2D list : a list of lists
numbers = [ 
    [1,2,3], 
    [4,5,6],
    [7,8,9]
]

print(numbers[2][0])
print(numbers[1][1])
print(numbers[0][2])

for row in numbers: # in ra từng hàng trong list
    print(row)
print("\n")

for row in numbers: # in ra từng phần tử trong list
    for element in row:
        print(element, end=" ")
    print()
#----------------------------------------------------------------------------------------#
# 17 tuple : giống list 
# sự khác biệt với list là : list cho phép thêm xóa . sửa còn tuple thì không 

# tuple = (1,2,3,4,5) # example
# print(tuple)
# bro = ("mel", 21, "male")

# print(bro.count("mel")) # đếm số lần xuất hiện của phần tử trong tuple
# print(bro.index("male")) # trả về vị trí của phần tử trong tuple 0,1,2

# for x in bro:
#     print(x)   

# if 1 in bro:
#     print(1) # kiểm tra xem phần tử có trong tuple không nếu có in ra
# else:   
#     print("not here") # nếu không có thì in ra not here
#----------------------------------------------------------------------------------------#
# 18 set : là một tập hợp không có thứ tự và không thể thay đổi vì set kh cho phép các phần tử trùng lặp

food = {"hamberger", "pizza", "hotdog", "spaghetti"}
desert = {"ice cream", "pudding", "cake" , "hotdog", "spaghetti"}
drinks = {"soda", "water", "juice"}
result = food.union(desert , drinks) # gộp 3 set lại với nhau
print(result)
print(food.difference(desert)) # trả về các phần tử không trùng lặp
print(food.intersection(desert)) # trả về các phần tử trùng lặp

# food.add("rice")
# food.remove("pizza")
# food.clear() # xóa toàn bộ set
# hàm union : gộp 2 hoặc nhiều set lại với nhau
# food.update(desert) # thêm 1 set vào 1 set khác
# for x in food: 
#     print(x)


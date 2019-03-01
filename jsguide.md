# BASICS 

> **Luôn nhớ:** thêm **`'Use strict';`** vào đầu file JS

## Statements

Một ***chương trình(program)*** là một tập các ***chỉ thị(intructions)***  
Các ***chỉ thị(intructions)*** này sẽ được ***thực thi(executed)*** bởi máy tính  

***Ngôn ngữ lập trình(programming language)*** coi các ***chỉ thị(intructions)*** này là các ***câu lệnh(statements)*** 

***Câu lệnh(statement)*** có chức năng thực hiện một hành động nào đó  
Một ***câu lệnh(statement)*** được kết thúc bằng dấu chấm phẩy **;**  

&nbsp; &nbsp;&nbsp; <\<**a statement**>\> **;**
 
```js
alert("This is a statement");
```


Các ***câu lệnh(statements)*** được thực hiện tuần tự, từ ***trái sang phải***, từ ***trên xuống dưới*** 

Các ***câu lệnh(statements)*** có thể được nhóm với nhau trong một ***khối lệnh(code block)*** bằng 2 dấu ngoặc nhọn ***{...}***


## Values

Javascript có 2 kiểu ***giá trị(value)*** :   ***Fixed values(literals)*** và ***Variable values(variables)***  

### Literals
&nbsp; &nbsp;&nbsp; ***Literals*** có nghĩa là ***các giá trị thể hiện chính nó***  
&nbsp; &nbsp;&nbsp; ***Literals*** là giá trị cố định, không thể bị thay thế

```js
100 // 100(number) is a literal
"This is literal" // this string is a literal
```

### Variable
***Biến(variable)*** được sử dụng để lưu trữ dữ liệu (cho một ***giá trị(value)***)

***Biến(variable)*** đặt tên cho một ***giá trị(value)***, ***giá trị(value)*** được thể hiện qua các ***kiểu dữ liệu(data types)*** 

***Biến(variable)*** có thể lưu trữ(hold) mọi thứ, mọi kiểu dữ liệu

Javascript sử dụng ***từ khóa(keyword)*** `let` để ***khai báo(declares, hoặc defines)*** một ***biến(variable)***

> ***Các từ khóa(keywords)*** sử dụng để tạo nhãn cho hành động muốn thực thi

***Toán tử gán(assignment operator)***: dấu ***=*** được sử dụng để ***gán(assign)*** một ***giá trị(value)*** cho một ***biến(variable)***
> Công việc này còn được gọi là ***Khởi tạo giá trị cho một biến(Initializing a variable)***

```js
let myAge; //biến myAge được khai báo;
myAge = 24; //biến myAge được gán giá trị là 100(kiểu number)

/* myAge là 1 biến
   24 là giá trị của biến myAge
*/
```
***The right way:*** 

```js
let myAge = 24;  
```

***Truy cập(access)*** tới một ***biến(variable)*** bằng tên của nó
```js
alert(myAge);
```

Thay đổi giá trị của một biến
```js
let myAge = 24;
myAge = 20; //value changed form 24 to 20, value 24 removed
```

### Constant
***Hằng(constant)*** là giá trị không thay đổi
```js
const NUMBER = 100;
```

### Expression

Một đoạn mã code thực thi và tính toán(trả về - return) để ra một ***giá trị(value)*** mới thì được gọi là một ***biểu thức(expression)***

***Literal*** là một ***expression*** 
```js
142 //a number, also a literal, also a expression
"My name is An" //a string, also a literal, also a expression 
```

Các phép tính toán là một ***expression***
```js
5 + 6
"My name is" + "An"
```

Các ***expression*** có thể lồng nhau để tạo thành một ***expression*** 
```js
a = 5
myAge = 20
```

Khi một ***expression*** có thêm dấu **;** thì nó còn được gọi là ***câu lệnh biểu thức(expression statement)***
```js
a = 5 //expression
a = 5; //now is expression statement

alert(1) //expression
alert(1); //now is expression statement
```

> ***expression statement*** là kiểu phổ biến nhất


```js
let a = 100,
    b = 50;
    
if (a > b) {
  alert("a lớn hơn b");
}
```
**Trong đó :**
```js 
a
```
là một ***định danh(indentifier)*** của ***biến(variable)*** `a`

```js 
100;
50;
```
là các ***Literals*** (không thể thay đổi)
```js 
let a = 100, 
    b = 50;
```
là một ***khai báo(Variable Declaration)***

```js 
(a > b) //binary expression
alert("a lớn hơn b")
```
là các ***biểu thức(expressions)***

```js 
alert("a lớn hơn b");
```
là một ***câu lệnh biểu thức(expression statement)***

### Câu lệnh Return

***Trả về(return)*** là hành động trả về giá trị của 1 biểu thức tính toán

Lệnh ***trả về(return)*** sẽ yêu cầu chương trình dừng dòng lệnh và ***trả về(return)*** giá trị của ***biểu thức(expression)***

### Identifier

***Định danh(indentifiers)*** chính là các ***tên(names)*** sử dụng để đặt tên cho ***biến(variable)***, ***từ khóa(keyword)***, ***hàm(function)***,...

Đặt tên ***định danh(indentifier)*** bằng các nguyên tắc: 
* ***Tên(hay Định danh)*** chỉ được phép chứa **chữ cái**, **chữ số**, và 2 ký tự đặc biệt là **$** và **_** 
* Chữ cái bắt đầu **<span style="color:red">không</span>** được phép là chữ số


> **Javascript có phân biệt chữ in hoa và in thường**


### Comments
Có 2 kiểu comment
* Một dòng: //
* Nhiều dòng: /*
&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;\*/

> **Javascript bỏ qua việc xử lý comments**


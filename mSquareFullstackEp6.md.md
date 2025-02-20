﻿
## MSquare Programing Fullstack Course

### Episode-6 Summary

ဒီနေ့မှာတော့ JavaScript Function အကြောင်း လေ့လာသွားကြမှာပါ။၊<br>
 `function` တွေကို အချိန် နဲ့ နေရယူတာကို လျော့နည်းစေရန်၊ တူညီတဲ့လုပ်ဆောင်ချက်များကို ထပ်ခါထပ်ခါ ရေးစရာမလိုပဲ  တစ်ခါသတ်မှတ်ထားရုံနဲ့ ပြန်လည်ပြီး အကြိမ်ကြိမ် အသုံးပြုနိုင်ရန်၊ စတာတွေအတွက် အသုံးပြုကြပါတယ်
![enter image description here](https://res.cloudinary.com/practicaldev/image/fetch/s--pClJgvrv--/c_limit,f_auto,fl_progressive,q_auto,w_880/https://dev-to-uploads.s3.amazonaws.com/i/mt2jlra7jd5gdgl8up8y.png)


#### JavaScript မှာ function ကို အသုံးပြုမယ်ဆိုရင်

 1. function ကို အရင် သတ်မှတ် ပေးရပါမယ် (define, declare)
 2. ထို သတ်မှတ်ထားတဲ့ function ကို အသုံးပြုရန် / အလုပ်လုပ်စေရန် function ကို ပြန်လည်ခေါ်ယူ ပေးရပါမည်။(call)
  
  ##
  ### Function တစ်ခု သတ်မှတ်ခြင်း (define, declare)
  - ပထမနည်းလမ်း<br>
syntax<br>
      ``function-keyword`` ``functionနာမည်`` ( ``parameter`` ){
       ``function body ;``
       } ;

  <br> code

     function helloWorld(){
        console.log("Hello world");
        };

- **ES6 arrow Function** (anonymous အမည်မဲ့)<br>
syntax<br>
   `(parameter)` `=>` `{`
   `function body;`
   `}`
<br>
code
   

     () => {
        console.log (" Hello world");
        };

 **ES6** function ကို variable တစ်ခုထဲတွင် သိမ်းထားလေ့ရှိပါတယ်။<br>
code

    const sayHello = () =>{
    console.log ( " Hello ")
    } ;
         
##
### Function ကို ခေါ် ယူအသုံးပြုခြင်း
အထက်မှာ ဖော်ပြခဲ့သလို function တွေကို သတ်မှတ်လိုက်ရုံ နဲ့ ဘာ လုပ်ဆောင်ချက်မျှ
ပြုလုပ်ပေးမည်မဟုတ်ပါ။<br>
သတ်မှတ်ထားတဲ့ **function Name** (or) **သိမ်းထားတဲ့ variable Name** ကို **ခေါ််ပေးမှသာ** function က အလုပ်လုပ်မည်ဖြစ်သည်။

    
      function helloWorld(){
        console.log("Hello world");
      };
       helloWorld();//call by function name
      
      //Hello world

**ES6**
   

       const sayHello = () =>{
         console.log ( " Hello ")
       } ;
            sayHello();//call by variable name
            
            // Hello
##
### **Function with parameter**
 - function name နောက်က လက်သဲကွင်း ထဲမှာ parameter ကို ထည့် သွင်းကာ define လုပ်နိုင်သည်။
 - ထို function ကို ခေါ် သုံးသောအခါ နောက်က လက်သဲကွင်း ထဲမှာ parameter ရဲ့ တန်ဖိုးကို ထည့် သွင်း
 ပြီး အသုံးပြုနိုင်ပါသည်။

code

    //example - 1
    
    function sayHi(name) {
    console.log ( "Hi" + " ," + name);
    };
    
    sayHi("Mg Mg");
    // Hi ,Mg Mg
    
    sayHi ("Su Su");
    // Hi ,Su Su
    
    example -2
    
    function numberPlus(a,b){
    console.log ( a + b );
    };
    numberPlus(2,5);
    // 7
    numberPlus(80,160);
    // 240

 
 ### ES6
 

    //example - 1
    
     const helloUser = (name) =>{
        console.log ( "Hello" + " ," + name);
        };
        
     helloUser("Mg Mg");
    // Hello ,Mg Mg
    
     helloUser("Su Su");
    // Hi ,Su Su
    
    //example -2
    
    const multipleNumber = (a,b)=>{
      console.log ( a * b );
    };
    
     multipleNumber(2,5);
    // 10
    
     multipleNumber(80,160);
    // 12800
##
### Return
 - function များ၏ လုပ်ဆောင်ချက်**ရလဒ် များကို ရယူအသုံးပြုနိုင်ရန်** return ဖြင့် ထုတ်ပြန်ပေးရသည်။
မှတ်ချက်။ ။ **console.log သည်** ရလဒ်ကို အသုံးပြုနိုင်ရန် ထုတ်ပေးခြင်း မဟုတ်ပါ။ <br>
**console ထဲတွင် log တစ်ခုအနေနဲ့ ပြသပေးရုံသာ** ဖြစ်သည်။
 
 - function များကို **return မပေးထားရင် Undefined** ဟူသော တန်ဖိုး
   ပြန်ထုတ်ပေးသည်။

 
  

     const toCheck = (a,b) => {<br>
             return (a + b );<br>
             }<br>
             toCheck( 3, 4);<br>
             //return 7

### Try this ....

    const cake = 5;
    const juice = 3;
    const orange = 1;
    const apple = 4;
    const dragon = 4000;
    const discountPrice = 1;
    let normalPrice;
    let toPay;
    
      const totalPrice = ( price1 , price2)=> {
       normalPrice = price1 + price2 ;
       return normalPrice;
     }
     totalPrice( cake , juice);
    
   
    const haveToPay = ( a , b) => {
     toPay = a - b ;
     return toPay ;
    };
    haveToPay(normalPrice,discountPrice);
    
    console.log ( "You Have to Pay " + toPay + "$"+" "+ "Total");
    // You Have to Pay 7$ Total

       
**totalPrice** function ခေါ််တဲ့အခါ  **parameter** တွေမှာ အခြားတန်ဖိုးတွေ ( orange , apple, dragon) အစားထိုးပြီး **console မှာ run** ကြည့်ပါ။

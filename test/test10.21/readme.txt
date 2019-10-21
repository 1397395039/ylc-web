1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:    
       var h1 = document.getElementById('h1');
       var str="Hello";
       var str2="world";
       var str3=str.concat(str2);
       h1.innerHTML=str3;

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:
        var h2 = document.getElementById('h2');
        var str = "87";
        h2.innerHTML=str.padEnd(6,'0');

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:
        var h3 = document.getElementById('h3');
        var str = "79387.348";
        var str2 = Number.parseFloat(str);
        h3.innerHTML=str2.toFixed('2');
       
4.一张图片是一个相对路径img/head/icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:
         var h4 = document.getElementById('h4');
         var imgs = document.getElementsByTagName('img');
         var img1s = imgs[0].getAttribute('src');
         h4.innerHTML=img1s;

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h5的元素中
答:     
         var h4 = document.getElementById('h4')
         var c ='eXtc';
         var a = prompt("请输入验证码（eXtc）")
         var b = a.toLowerCase();
         var d = c.toLowerCase();
         if(d==b){
            h4.innerHTML = b;
         }else{
             alert('输入验证码错误')
         }
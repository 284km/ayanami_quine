
ayaanmi_quine
=============


```
$ less ayanami_quine.rb
eval$s=%w'b="BAhsKwGGAAAA/B8AAAAAAAAAwP//DwAAAAAAAPjvf/4CAAAAAADoe3e+AAAAAAAArE/+ywAAAAAAAADrPwQAAAAAAAAAOA0DAAAAAAAAAACHfwAAAAAAAACAI/wPAAAAAAAAwAXsHwAAAAAAAHAA8QMAAAAAAAAQAMR0AAAAAAAAxobFBgAAAAAAQDDA/n8AAAAAABAO+P9/AAAAAABmAP7//w8AAADAQAD8////AQAA+CAB/v///wcAAHBXgP////8BAED/H/D///8/AAAQ/4f/////AwAAIABA/P//Pw8AByBMkP//Z/z/bQNAAED+//z/NwAAQAOA5///u8lwIwBoIThIM0AJBgAAAAAAAAAADA==";n=Marshal.load(b.unpack("m")[0]);e="eval$s=%w"<<39<<($s*3);o="";j=-1;0.upto(27*80-1){|i|o<<((n[i]==1)?e[j+=1]:32);o<<((i%80==79)?10:"")};o[-10,6]=""<<39<<".join";puts(o)#'.join
```

It's work !!

```
$ ruby ayanami_quine.rb | ruby | ruby
                          eval$s=%w'b
                      ="BAhsKwGGAAAA/B8AAAAA
                   AAAAwP//D wAAAAAAAPj  vf/4CAA A
                   A AADoe 3e+A AAA AAA  ArE/+ y
                  wA A AAAAA  A  DrPwQAAAA A  AA
                        AA O A0DAAAAAA    A
                           AAA  C Hf    wA
                                AAA    AAAACAI/
                               wPA   A    AAAAAAwAXs
                              HwA A       AA AAAHAA8Q
                            MAA         A   AAAAAQ
                            A             M   R0  A AAA
                         AA   AA xo    bF B   gA AA
                      A     AA        QD DA/n8AAAAAABAO
                    +    P9/       AAAAAABmAP7//w8AAADA
                 QA  D8          ////AQAA+CAB/v///wcAAHBXgP/
              //      /           8BAED/H/D///8/AAAQ/4f/////AwAAI
           ABA/P     /  /        Pw8AByBMkP//Z/z/bQNAAED+//z/NwAAQA
            OA5 /// u 8        lwIwBoIThIM0AJBgAAAAAAAAAADA==";n=
      M arshal.load(b       .unpack("m")[0]);e="eval$s=%w"<<39
    <   <($s*3);o="    ";j=-1;0.upto(27*80-1){|i|o<<((n[i]
     =                =   1)?e[j+=1]:32);o<<((i%80==79  )?10            :""
     )    };  o     [  -10,6]=""<<39<<".joi  n"   ;puts(o)#b="BAh sK wG GA
      A               A  A/B8AAAAAAAAAwP  //DwAAAAAAAPjvf/4 CA
      A AA             AADo  e3e+AAAAAAAArE/+ywAAA AAA AA  D  rP    wQA AA   A
           A AA A    A     OA0     D  A AA  AA        A A  A     AA
```
 

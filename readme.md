# minifsharp
顾名思义，小的F#，是本人在武汉肺炎的时候无聊搞的一种船新的语言，全名minifsharplang。
语法糖优美简单深得我心。
```f#

let createdict k,v,m,n = {
    {k,v;m,n};
}

let mydict = createdict "a","2","b","4";

mydict.a |> print;
mydict.b |> print;

let dict2 = {"m",1;"n",2};
dict2.m |> print;
dict2.n |> print;

let readfile path = {
    let p = ["read", "read2"];
    path |> file.[p.["0"]] |> print;
    p.["1"] |> print;
    path |> file.[p.["0"]];
}

readfile "./test.txt" |> print;

let v = readfile "./test.txt";

if v {
   print v;
} else {
   print 2,(4+1),4;
}
```
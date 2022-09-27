### 基本数据类型
const hd:string = '';

const hd:number = 100;

const hd:boolean = true;

### 数组
let hd:Array<string> = [];
hd.push('1', '2);

let hd = new Array<string>(3).fill('7');
console.log(hd);

- 明确数组每个成员类型的数组为元组
let hd:[string, number, boolean];
hd = ['1', 10, true];
console.log(hd);

### 对象
- 声明对象类型但不限制类型
let obj:object;0
hd = { name: 'hd' };
hd = {}; // 字面量声明对象
hd: []; // 数组也是对象
hd = Object.prototype; // 原型对象
hd = '123'; // 报错

- 限定对象值类型
let hd:{ name: string, year:number };
hd = { name:'后盾人', year:2010 }

- 属性后面跟上?用来指定url为可选值，这样的属性是非必填项
let hd:{ name: string, year:number, url?:string }
hd = { name:'后盾人', year:2010 };

### any
- any包含所有制的顶部类型，不进行类型监测
let hd:any;
hd = '123';

let hd:any[] = ['123', 123 true];
let hd:Array<any> = [123, '123', true];

let hd: {
    name: any,
    year: any,
}
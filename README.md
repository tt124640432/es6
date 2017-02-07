### 默认导入和命名导入 
1. import theDefault,{named1,named2} from './libs/index'
2. import theDefault from './libs/index
3. import {named1,named2} from './libs/index'

### 重命名
import {named1 as myname1,named2} from './libs/index'
### 导入模块为对象
import * as mylibs from './libs/index'

### 只导入文件
import './libs/index';

### 命名导出和默认导出
export const named1 = {}
export default function() {}

### 将本身内容导出
const my_const = '123';
function myFn(str) {
    return str.split('').join('-')
}
export { my_const, myFn }

### 导出的时候给他们改个名字
export { my_const as test_const,myFn as testFn }

### 还可以导出从其他地方导入的模块
export * from './libs/other';
export { foo, bar } from './libs/other';
export { foo as myFoo, bar } from './libs/other';

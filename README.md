<p align="center">
  <a href="http://www.xuxuepu.com">
    <img width="100" src="http://7xk0ie.com1.z0.glb.clouddn.com/123.jpg/min100">
  </a>
</p>

# 正则校验

## 特性

- 用于表单正则校验

## 安装

```
npm install xxp-verification
```

## 示例

```
import xv from 'xxp-verification';
//判断邮箱格式是否正确
let isEmail = xv.checkEmail('xxp@qq.com');
console.log(isEmail);//正确返回true，否则返回false
```

## 方法

```
isIP(strIP)//用途：校验ip地址的格式  输入：strIP：ip地址  返回：如果通过验证返回true,否则返回false；
isNull(str)//用途：检查输入字符串是否为空或者全部都是空格 输入：str 返回： 如果全是空返回true,否则返回false
isBankCard(str)//验证银行卡号
isBillphone(str)//验证发票号码格式
isInteger(str)//用途：检查输入对象的值是否符合整数格式 输入：str 输入的字符串 返回：如果通过验证返回true,否则返回false
checkPrice(s)//城市价格校验 (小于1000的整数 或者只有两位小数的浮点数)
checkZnumber(s)// 小于1000的整数
checkMobile(s)//用途：检查输入手机号码是否正确 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isNumber(s)//用途：检查输入字符串是否符合正整数格式 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isDecimal(str)//用途：检查输入字符串是否是带小数的数字格式,可以是负数 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isPort(str)//用途：检查输入对象的值是否符合端口号格式 输入：str 输入的字符串 返回：如果通过验证返回true,否则返回false
isEmail(str)//用途：检查输入对象的值是否符合E-Mail格式 输入：str 输入的字符串 返回：如果通过验证返回true,否则返回false
isMoney(s)//用途：检查输入字符串是否符合金额格式 格式定义为带小数的正数，小数点后最多三位 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isNumberOr_Letter(s)//用途：检查输入字符串是否只由英文字母和数字和下划线组成 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isNumberOrLetter(s)//用途：检查输入字符串是否只由英文字母和数字组成 输入： s：字符串 返回： 如果通过验证返回true,否则返回false
isChinaOrNumbOrLett(s)//用途：检查输入字符串是否只由汉字、字母、数字组成 输入： value：字符串 返回： 如果通过验证返回true,否则返回false
isDate(date, fmt)//用途：判断是否是日期 输入：date：日期；fmt：日期格式 返回：如果通过验证返回true,否则返回false
getMaxDay(year, month)
isLastMatch(str1, str2)//用途：字符1是否以字符串2结束 输入：str1：字符串；str2：被包含的字符串 返回：如果通过验证返回true,否则返回false
isFirstMatch(str1, str2)//用途：字符1是否以字符串2开始 输入：str1：字符串；str2：被包含的字符串 返回：如果通过验证返回true,否则返回false
isMatch(str1, str2)//用途：字符1是包含字符串2 输入：str1：字符串；str2：被包含的字符串 返回：如果通过验证返回true,否则返回false
checkTwoDate(startDate, endDate)//用途：检查输入的起止日期是否正确，规则为两个日期的格式正确， 且结束如期>=起始日期 输入： startDate：起始日期，字符串; endDate：结束如期，字符串 返回： 如果通过验证返回true,否则返回false
checkEmail(strEmail)//用途：检查输入的Email信箱格式是否正确 输入： strEmail：字符串 返回： 如果通过验证返回true,否则返回false
checkPhone(strPhone)//用途：检查输入的电话号码格式是否正确 输入： strPhone：字符串 返回： 如果通过验证返回true,否则返回false，7-8位的座机号(区号3-4位 可带可不带)或者 11位的手机号
checkSelect(checkboxID)//用途：检查复选框被选中的数目 输入： checkboxID：字符串 返回： 返回该复选框中被选中的数目
getTotalBytes(varField)
getFirstSelectedValue(checkboxID)
getFirstSelectedIndex(checkboxID)
selectAll(checkboxID, status)
selectInverse(checkboxID)
checkDate(value)
checkPeriod(startDate, endDate)用途：检查输入的起止日期是否正确，规则为两个日期的格式正确或都为空 且结束日期>=起始日期 输入： startDate：起始日期，字符串 endDate：结束日期，字符串 返回： 如果通过验证返回true,否则返回false
checkSecCode(secCode)//用途：检查证券代码是否正确 输入： secCode:证券代码 返回： 如果通过验证返回true,否则返回false
```

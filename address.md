#1、生成随机数
##例如：
  ```用户id + salt ----Sha256---->  sha1
  sha1 + salt  ----Sha256---->  sha2
  sha2 + salt  ----Sha256---->  sha3
  sha3 做hex处理生成随机数seed
  ```
#2、生成根私钥 
  ```
  用seed生成私钥以及hd钱包
  ```
#3、生成path
 ```
  https://github.com/satoshilabs/slips/blob/master/slip-0044.md
  根据以上规则通过用户索引生成path
  ```
#4、根据根私钥与path生成子私钥
  ```
  通过hd钱包由根私钥+ path生成子私钥(用户私钥)
   ```


## 🔹 What is Subnetting?

**Subnetting = dividing one network into multiple smaller networks**

###  Why?

- Better network performance
- Reduced congestion
- Efficient IP usage
- Security (isolation)

###🔹 How to Calculate Subnets (IMPORTANT 🔥)

####  Step 1: Know the Formula

##### ✔ Number of Subnets:

```
2^n
```

 n = borrowed bits

##### ✔ Number of Hosts:

```
2^h - 2
```

 h = host bits
  (-2 for network & broadcast)

# 🔹 Example (Easy)
 Network:

```
192.168.1.0/24
```

 Suppose we borrow 2 bits:

 New subnet mask:

```
/26
```


##### 🔸 Calculate Subnets:

```
2^2 = 4 subnets
```
##### 🔸 Calculate Hosts per Subnet:

```
2^6 - 2 = 62 hosts
```

##### 🔸 Subnet Ranges:

| Subnet | Range               |
| ------ | ------------------- |
| 1      | 192.168.1.0 – 63    |
| 2      | 192.168.1.64 – 127  |
| 3      | 192.168.1.128 – 191 |
| 4      | 192.168.1.192 – 255 |



### 🔹 Useful Tools
 You can use these tools to calculate subnetting:

* **ip Subnet Calculator** (https://www.calculator.net/ip-subnet-calculator.html)
* **Art of infra** (https://calc.artofinfra.com/)

-  Just enter IP + CIDR → it gives:

* Network ID
* Broadcast
* Host range
* Subnets
* 
###### Final Summary

✔ Subnet = smaller network
✔ Subnet mask = defines network & host
✔ CIDR = shorthand notation
✔ Subnetting = dividing network
✔ Use formulas to calculate subnets & hosts


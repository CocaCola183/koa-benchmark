# koa-benchmark

比较koa和koa2和express性能

## Prerequisites

for OSX

```
brew install wrk
```

## Test

首次测试，需要安装依赖，会比较慢

```
make all
```

不安装依赖，重复测试

```
make test
```

## Results

```
➜  koa-benchmark git:(master) ✗ node -v
v4.0.0
➜  koa-benchmark git:(master) ✗ npm -v 
2.14.2
➜  koa-benchmark git:(master) ✗ npm test 
benchmark koa-1

  1 middleware
  5976.88

  5 middleware
  3495.61

  10 middleware
  5494.52

  15 middleware
  5444.90

  20 middleware
  5631.77

  30 middleware
  5091.48

  50 middleware
  3657.46

  100 middleware
  4712.93
  
benchmark koa-2

  1 middleware
  5959.41

  5 middleware
  5653.19

  10 middleware
  5652.32

  15 middleware
  5882.88

  20 middleware
  5929.52

  30 middleware
  5700.04

  50 middleware
  5852.57

  100 middleware
  5211.41

benchmark express

  1 middleware
  5500.16

  5 middleware
  5783.63

  10 middleware
  5561.32

  15 middleware
  5253.31

  20 middleware
  5305.64

  30 middleware
  4950.02

  50 middleware
  4472.47

  100 middleware
  4077.43
  
```
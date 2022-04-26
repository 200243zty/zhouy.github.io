---
title: 你好，世界！
date: 2022-03-26 10:34:00 +0800
categories: [随笔]
tags: [生活]
pin: true
author: 湾区书记汤姆

toc: true
comments: true
typora-root-url: ../../tomstillcoding.github.io
math: false
mermaid: true

image:
  src: /assets/blog_res/2021-03-30-hello-world.assets/huoshan.jpg
  alt: 签约成ar
---

# start

快速排序

```c++
void quick_sort(int q[],int l,int r){
    if(l>=r) return ;
   	int i=l-1,j=r+1,x=q[l+r>>1];
    while(i<j){
		do i++;while(q[i]<x);
         do j--;while(q[j]>x);
        if(i<j) swap(q[i],q[j]);
    }
    quick_sort(q,l,j);quick_sort(q,j+1,r);
}
```


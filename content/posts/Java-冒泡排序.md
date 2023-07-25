---
title: Java-冒泡排序
date: 2020-07-20 21:00:24
updated: 2020-07-20 21:00:24
toc: true #是否显示文章目录
math: true
excerpt: Java版冒泡排序(待优化)
index_img: https://online-education-headimg.oss-cn-beijing.aliyuncs.com/%E5%8D%9A%E5%AE%A2/%E5%85%AC%E5%85%B1%E5%9B%BE%E7%89%87%E8%B5%84%E6%BA%90/post_default_img.png
categories: [排序算法] #分类
tags: [Java] #标签
---



# Java-冒泡排序



## 简要说明

依次比较两个相邻的元素



## 动图展示

![冒泡排序](https://online-education-headimg.oss-cn-beijing.aliyuncs.com/%E5%8D%9A%E5%AE%A2/%E5%8D%9A%E5%AE%A2%E6%96%87%E7%AB%A0%E5%9B%BE%E7%89%87/bubbleSort.gif)



## 代码展示

```java
public class BubbleSort {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		int[] arr = {3, 44, 38, 5, 47, 15, 36, 26, 27, 2, 46, 4, 19, 50, 48};
		
		for (int i = 0; i < arr.length - 1; i++) {
			for (int j = 0; j < arr.length - i - 1; j++) {
				if (arr[j] > arr[j + 1]) {
					int temp = arr[j];
					arr[j] = arr[j + 1];
					arr[j + 1]  = temp;
				}
			}
		}
		System.out.println(Arrays.toString(arr));

	}

}

```

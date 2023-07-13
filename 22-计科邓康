package main

import (
	"fmt"
	"sort"
	"strings"
)

func sortSubarray(arr []int, l int, r int) {
	subarray := arr[l : r+1]
	sort.Ints(subarray)
	for i := l; i <= r; i++ {
		arr[i] = subarray[i-l]
	}
}

func main() {
	var n, l, r int
	fmt.Scan(&n, &l, &r)

	arr := make([]int, n)
	for i := 0; i < n; i++ {
		fmt.Scan(&arr[i])
	}

	sortSubarray(arr, l, r)

	fmt.Println(strings.Trim(fmt.Sprint(arr), "[]"))
}

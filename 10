package main

import "fmt"

func Pares(s []int) map[int]int {
	frequenciaS := make(map[int]int)

	for _, ranS := range s {
		frequenciaS[ranS] += 1
	}
	for numero, frequencia := range frequenciaS {

		if frequencia%2 != 0 {
			delete(frequenciaS, numero)
		} else {
			frequenciaS[numero] /= 2
		}
	}
	return frequenciaS
}

func main() {
	s := []int{3, 2, 1, 9, 4, 2, 5, 1, 3, 4, 9, 5, 4}

	fmt.Println(Pares(s))
}

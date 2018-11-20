# Java
Códigos em JAVA  

Exercício Busca em  Java

public static int buscaBin(int[] v, int e) {
		int setaMenor=0, setaMaior = v.length-1,mid = (setaMenor+setaMaior)/2;
		while(setaMenor <= setaMaior) {
			mid = (setaMenor+setaMaior)/2;
			if(v[mid]<e) {
				setaMenor=mid+1;
			} else if(v[mid]>e) {
				setaMaior=mid-1;
			} else {
				return 1;
			}
		}
		return 0;
	}
	
	public static int buscaBinIndice(int[] v, int e) {
		int setaMenor=0, setaMaior = v.length-1,mid = (setaMenor+setaMaior)/2;
		while(setaMenor <= setaMaior) {
			mid = (setaMenor+setaMaior)/2;
			if(v[mid]<e) {
				setaMenor=mid+1;
			} else if(v[mid]>e) {
				setaMaior=mid-1;
			} else {
				return mid;
			}
		}
		return -1;

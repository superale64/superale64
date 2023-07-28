
Public Class Matrices
    'Función para sumar matrices
    Function SumaMatrices(matriz1(,) As Integer, matriz2(,) As Integer) As Integer(,)
        Dim matrizResultante(,) As Integer = matriz1

        For i As Integer = 0 To matriz1.GetLength(0)-1
            For j As Integer = 0 To matriz1.GetLength(1)-1
                matrizResultante(i, j) = matriz1(i, j) + matriz2(i, j)
            Next
        Next

        Return matrizResultante
    End Function

    'Función para restar matrices
    Function RestaMatrices(matriz1(,) As Integer, matriz2(,) As Integer) As Integer(,)
        Dim matrizResultante(,) As Integer = matriz1

        For i As Integer = 0 To matriz1.GetLength(0)-1
            For j As Integer = 0 To matriz1.GetLength(1)-1
                matrizResultante(i, j) = matriz1(i, j) - matriz2(i, j)
            Next
        Next

        Return matrizResultante
    End Function

    'Función para imprimir la matriz resultante
    Function ImprimirMatriz(matriz(,) As Integer) As String
        Dim result As String = ""

        For i As Integer = 0 To matriz.GetLength(0)-1
            For j As Integer = 0 To matriz.GetLength(1)-1
                result += matriz(i, j).ToString() + " "
            Next
            result += Environment.NewLine
        Next

        Return result
    End Function
End Class

superale64/superale64 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

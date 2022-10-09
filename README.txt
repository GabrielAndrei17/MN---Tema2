Andrei Gabriel - 323CB
Tema 2 - Interpolare aplicata pe imagini

1. Bicubic:

	functia precalc_d primeste ca parametru imaginea I apoi cu ajutorul functiilor
auxiliar fy, fx si fxy se calculeaza matricile cu derivate.

	functia bicubic_coef calculeaza coeficientii de interpolare bicubica pentru 4 puncte alaturate,
valori ce se retin in matricea finala A, care se calculeaza astfel A = M_const1 * M * M_const2;

	functia bicubic_resize calculeaza punctele ce inconjoara punctul (x, y),
apoi se calculeaza coeficientii de interpolare cu ajutorul functiei bicubic_coef.
Valoarea interpolata a pixelului se calculeaza dupa formula data.

2. Proximal:

	functia proximal_2x2 primeste ca parametrii imaginea si numarul de pasi
apoi itereaza prin numarul de puncte si completeaza matricea finala folosind
formula prezentata.

	functia proximal_coef - calculeaza coeficientii pentru interpolarea proximala 
intre punctele (x1, y1), (x1, y2), (x2, y1) si (x2, y2). Se foloseste matricea
A, apoi coeficientii se retin in vectorl a.

	functia proximal_resize - asemanator cu bicubic_resize.

	functia proximal_rotate - calculeaza cosinusul si sinusul unghiului primit ca parametru,
apoi se aplica ca mai devreme matricea de transoformare si inversa sa. 
Apoi calculam coeficientii de interpolare si valoarea interpolata a punctului.

3. Lanczos:

  
  

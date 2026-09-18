# Labo suite de Wallis (pseudo code)

user_numerator <- saisie utilisateur
user_denominator <- saisie utilisateur

si user_numerator mod 2 != 0 ou user_denominator mod 2 != 1 ou user_numerator - user_denominator != 1 
    refaire taper à l'utilisateur

sinon 

numerator <- 0
denominator <- 1
counter <- 1
result <- 1

Tant que numerator != user_numerator et denominator != user_denominator

    counter <- counter + 1

    si counter mod 2 = 0
        numerator <- numerator + 2
    sinon 
        denominator <- denominator + 2

    result = result * (numerator / denominator)

fin tant que

afficher result
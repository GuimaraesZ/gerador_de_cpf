Projetos Utilitários 🛠️
Este repositório contém dois scripts em Python com propósitos distintos e educativos:

Cálculo do segundo dígito do CPF

Jogo de adivinhação de palavra

📌 1. Cálculo do segundo dígito do CPF
Descrição
Script que valida o CPF completo (incluindo primeiro e segundo dígito verificador) informando se é válido ou não, com foco no cálculo do segundo dígito.

Como usar
Execute o script:

bash
Copiar
Editar
python cpf_segundo_digito.py
Insira o CPF no formato com ou sem pontuação, por exemplo:
746.824.890-70

O script remove caracteres não numéricos, valida se não é sequência repetitiva e calcula os dígitos de verificação. Ao final, informa se o CPF é válido ou não.

Lógica aplicada
Remove ., - e espaços.

Verifica se os 11 dígitos não são todos iguais.

Calcula o primeiro dígito pelos 9 primeiros números.

Para o segundo dígito, utiliza os 9 primeiros + primeiro dígito, multiplicando-os pela contagem regressiva (11 a 2).

Multiplica o resultado por 10 e aplica mod 11.

Se o resultado for ≥ 10, atribui 0.

Compara o CPF informado com o CPF calculado.

🎯 2. Jogo de Adivinhação de Palavra
Descrição
Um "Hangman" simplificado: o usuário tenta descobrir uma palavra secreta, adivinhando letra por letra. Cada tentativa exibe acertos e a quantidade de tentativas realizadas.

Como usar
Execute o script:

bash
Copiar
Editar
python adivinhacao_palavra.py
A palavra secreta está pré-definida no código (perfume), mas pode ser alterada.

Digite apenas uma letra por vez. Se errar, um * é exibido no lugar da letra.

O jogo continua até a palavra completa ser descoberta.

Ao final, apresenta o número total de tentativas.

Lógica aplicada
Permite somente entrada de uma única letra.

Acumula as letras corretas em letras_acertadas.

Exibe a palavra com * em posições não descobertas.

Contabiliza e exibe o total de tentativas no fim.

Após vencer, limpa a tela e mostra mensagem de vitória

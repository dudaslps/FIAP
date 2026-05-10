Challenge Sprint 1 - Cognitive Cybersecurity
Grupo: Tropa de Elite
Turma: 1TIAPY

Como rodar o projeto:
1.	Abrir um terminal.
2.	Rodar o código python -m http.server 8000 –bind 127.0.0. .
3.	Com esse terminal ainda aberto, executar o script em um novo terminal.
Como roda o projeto:
Mediante passo a passo acima, o programa gera números aleatórios e tenta avisar um servidor. Se o servidor não estiver “ouvindo” (comando no item 2 do passo a passo), é exibido erro. 
O fluxo completo ocorre em três principais passos:
•	Sorteio de dados: o programa finge que é um sensor de trator e escolhe dados quaisquer de umidade e temperatura; 
•	Preparação do pacote: organiza os números em formato de texto padrão JSON e “empacota” tudo em bytes para que as informações possam trafegar na rede;
•	Tentativa de entrega: o programa tenta bater na porta do endereço específico 127.0.0.1:8000. Se a porta abrir, os dados são entregues. Caso contrário, é exibido aviso de que o servidor está desligado.

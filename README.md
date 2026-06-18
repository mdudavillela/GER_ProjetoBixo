# GER_ProjetoBixo
Projeto de seis semanas cujo objetivo é fazer um robô explorador.

- Semana 1: Estrutura e Mecânica
  - Cinemática diferencial (como girar duas rodas faz o robô curvar), conceito de centro de massa e boas práticas de modelagem 3D.
  - Objetivo: Projetar do zero o chassi do robô em um software CAD. Deve-se posicionar os motores de tração, a roda de apoio (caster) e garantir uma plataforma estável para a bateria e a eletrônica. O foco é desenhar tudo considerando a tolerância de encaixe físico e o equilíbrio de peso.

 - Semana 2: Eletrônica e Potência
   - Princípios de eletrônica de potência, pontes H, modulação PWM.
   - Objetivo: Montar a infraestrutura física e elétrica do robô. Deve-se realizar todas as soldas, crimpar conectores, ligar a bateria na ponte H e conectar o microcontrolador (ESP32) de forma segura. Precisa-se organizar os chicotes elétricos (cable management) para suportar vibrações sem desconectar.

- Semana 3: Odometria e Baixo Nível
  - Interrupções de hardware, leitura de encoders de quadratura e a cinemática de conversão de velocidade da rodas em posição no mundo (x, y, θ).
  - Objetivo: Programar o microcontrolador para ler as interrupções dos sensores das rodas em tempo real. Deve-se focar na calibração: girar o robô fisicamente, medir o deslocamento com uma trena na bancada e ajustar a matemática no código para que os "ticks" do encoder correspondam a metros por segundo reais.
 
- Semana 4: Controle de Movimento (PID)
  - Introdução à teoria de controle em malha fechada e os ganhos Proporcional, Integral e Derivativo (PID).
  - Objetivo: Implementar o algoritmo PID para que as rodas obedeçam fielmente aos comandos de velocidade. A equipe fará ciclos rápidos de "alteração de código > teste físico > análise", forçando o motor com as mãos (simulando atrito do chão) para sintonizar os ganhos e evitar que o robô oscile ou trema durante o deslocamento.

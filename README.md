# Doctor Sinta | Inteligência Artificial
Apresentamos a nova base de conhecimentos: Doctor Sinta. Desenvolvida para aprimorar diagnósticos médicos, utilizando o programa Expert Sinta. Este sistema é reconhecido no setor da saúde por sua capacidade de integrar dados clínicos e oferecer suporte decisivo a profissionais na tomada de decisões a partir de regras de conhecimento.

<p align="center">
  <img src="https://user-images.githubusercontent.com/91018438/204195385-acc6fcd4-05a7-4f25-87d1-cb7d5cc5c852.png" alt="animated" />
</p>

<center>
Group:

  
    Matheus Ryan | Lucas Heron
 </center>

## O que são Regras de Inferência?
Regras de inferência são princípios lógicos que permitem deduzir novas informações a partir de premissas já conhecidas. Elas são amplamente utilizadas em sistemas de lógica formal, inteligência artificial e programação de computadores. As regras podem ser expressas de várias maneiras, mas, geralmente, seguem um formato que conecta as premissas a uma conclusão.

## O que são Bases de Conhecimento?
Uma base de conhecimento é um sistema de armazenamento e recuperação de informações que permite a representação do conhecimento em um formato estruturado. É fundamental para a construção de sistemas especialistas, que tomam decisões com base em conhecimento pré-existente.

### Componentes de uma Base de Conhecimento
* Fatos: Informações que são consideradas verdadeiras. Exemplos incluem dados, definições e descrições.
* Regras: Instruções que definem como os fatos se relacionam e como novas informações podem ser deduzidas a partir deles.
* Ontologias: Estruturas que definem categorias, propriedades e relações entre conceitos dentro de um domínio específico.

## Regras de conheciemnto usadas no programa

### Diagnóstico de Diabetes (Versão Expandida)
* SE glicose em jejum > 126 mg/dL ENTÃO suspeita de diabetes.
* SE glicose em jejum > 126 mg/dL E glicose pós-prandial > 200 mg/dL ENTÃO pré-diagnóstico de diabetes.
* SE glicose em jejum > 126 mg/dL E glicose pós-prandial > 200 mg/dL E HbA1c > 6,5% ENTÃO diagnóstico de diabetes.
* SE glicose em jejum entre 100 mg/dL e 125 mg/dL OU HbA1c entre 5,7% e 6,4% ENTÃO pré-diabetes.
* SE glicose em jejum > 126 mg/dL E sintomas como sede excessiva, micção frequente e perda de peso inexplicada estão presentes ENTÃO diagnóstico de diabetes tipo 2.
* SE HbA1c > 6,5% E sintomas clínicos estão ausentes E histórico familiar de diabetes é positivo ENTÃO diagnóstico de diabetes, monitorar para possíveis complicações.
### Diagnóstico de Hipertensão (Versão Expandida)
* SE pressão arterial sistólica ≥ 140 mmHg OU diastólica ≥ 90 mmHg ENTÃO suspeita de hipertensão.
* SE pressão arterial sistólica ≥ 140 mmHg OU diastólica ≥ 90 mmHg E pressão permanece elevada em pelo menos duas medições diferentes em dias distintos ENTÃO pré-diagnóstico de hipertensão.
* SE pressão arterial sistólica ≥ 140 mmHg OU diastólica ≥ 90 mmHg E exames laboratoriais (colesterol, função renal) mostram alterações ENTÃO diagnóstico de hipertensão grau 1.
* SE pressão arterial sistólica ≥ 160 mmHg OU diastólica ≥ 100 mmHg E sintomas como dores de cabeça frequentes, tonturas e visão turva estão presentes ENTÃO diagnóstico de hipertensão estágio 2.
* SE hipertensão não controlada E exame de fundo de olho revela alterações vasculares OU sinais de hipertrofia ventricular esquerda no ECG ENTÃO hipertensão estágio 2 com complicações.
### Diagnóstico de Glaucoma (Versão Expandida)
* SE pressão intraocular (PIO) > 21 mmHg ENTÃO suspeita de glaucoma.
* SE PIO > 21 mmHg E há perda de visão periférica OU visão embaçada ENTÃO pré-diagnóstico de glaucoma.
* SE PIO > 21 mmHg E exame de campo visual mostra perda de visão periférica E exame do nervo óptico revela danos ENTÃO diagnóstico de glaucoma primário de ângulo aberto.
* SE PIO > 30 mmHg E danos ao nervo óptico estão avançados ENTÃO glaucoma avançado.
* SE paciente tem histórico familiar de glaucoma E está com PIO elevada, mas sem sintomas evidentes ENTÃO glaucoma em estágio inicial, recomendar monitoramento frequente.
* SE o paciente já foi diagnosticado com diabetes OU hipertensão E PIO > 21 mmHg ENTÃO risco elevado de glaucoma secundário.

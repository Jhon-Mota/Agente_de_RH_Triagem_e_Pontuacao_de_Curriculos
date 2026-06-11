# Agente de RH — Triagem e Pontuação de Currículos
## Descrição

Agente de IA desenvolvido no **N8N** para triagem automatizada de candidatos a vagas de TI. Analisa currículos enviados e atribui uma pontuação estruturada com base em critérios objetivos de experiência, formação e palavras-chave relevantes.

---

## Como funciona

1. O currículo do candidato é enviado por meio de um formulário.
2. É transformado em texto o currículo do candidato para posteriormente enviar para a IA.
2. O modelo analisa o documento com base em um prompt estruturado de RH
3. Uma pontuação é atribuída por categoria.
4. O resultado é retornado em formato JSON via **Structured Output Parser**.
5. Logo após, as informações (como nome, CPF, formação, pontuação total, etc.) do candidato são armazenadas em uma planilha do Google Sheets.

## Critérios de pontuação neste caso

| Experiência em TI (geral) | 3,0 |
| Experiência em Suporte / Help Desk / Infra / Redes | 4,0 |
| Empregado atualmente | 1,0 |
| Formação em TI — concluída | 1,5 |
| Formação em TI — em andamento | 0,75 |
| Cursos complementares (suporte, redes, infra) | 0,5 por curso |
| Palavras-chave (Suporte, TI, SQL, Hardware etc.) | 0,5 por palavra |
<br><br>

Workflow:<br>
<img width="1821" height="950" alt="Image" src="https://github.com/user-attachments/assets/70241fb5-a947-4429-b829-b02f163bee4a" /> <br><br>

Exemplo de cadastro na planilha:<br>:
<img width="1918" height="823" alt="image" src="https://github.com/user-attachments/assets/67ddc0a7-4a66-4434-a444-b3ac860b014a" /><br>
<img width="1916" height="934" alt="image" src="https://github.com/user-attachments/assets/9515d350-038d-4599-bd92-bb3b8f2202bd" />



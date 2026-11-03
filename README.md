# ClyvoVet — Compliance, Quality Assurance & Tests (Sprint 4)

Turma 2TDSPF

## Integrantes
- Mathaus Victor Souza Marcelino — RM564146
- Luan Peixoto Marins Rocha — RM562258
- Vinicius Luis Exposito Morasi Garcia — RM563340
- Eduardo Novaes Mollo — RM561515
- Carlos Alberto Guedes Neto — RM566022

## Entregas
- **Plano de testes manuais (Word):** `Plano_de_Testes_ClyvoVet.docx`
- **Testes automatizados (Katalon Recorder):** `ClyvoVet_Default_Suite_v5.krecorder`
- **Vídeo da configuração e execução dos testes:** https://youtu.be/CJi6GavKfEw
- **Repositório:** https://github.com/vinxlux/clyvosprint4 (branch `develop`)

## Sistema testado
ClyvoVet — https://clyvovet.vercel.app

## Casos de teste automatizados
| ID | Teste |
|---|---|
| TC01 | Login com credenciais válidas |
| TC02 | Login com credenciais inválidas |
| TC03 | Agendar consulta |
| TC04 | Cadastrar novo pet |
| TC05 | Prescrever medicamento |

O caso TC06 (acesso a página restrita sem login) foi executado somente de forma manual e está descrito no documento Word.

## Como executar a automação
1. Instalar a extensão **Katalon Recorder** no navegador (Chrome ou Firefox).
2. Abrir a extensão e importar o arquivo `ClyvoVet_Default_Suite_v5.krecorder`.
3. Executar a suite completa (**Play all**) na ordem: TC02, TC01, TC03, TC04, TC05.
   Os testes TC03 a TC05 usam a sessão aberta pelo login do TC01.
4. Conferir os resultados (verde = passou) no painel de log.

## Observações
- Os testes usam uma conta de teste e criam registros de demonstração no sistema.
- O microchip do TC04 é gerado automaticamente a cada execução para evitar duplicidade.

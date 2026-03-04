# 🔐 Sistema de Login com Validação (CLI)

Um simulador de sistema de autenticação via terminal construído em Python. Este projeto demonstra conceitos fundamentais de controle de acesso, validação de credenciais e gerenciamento de estado de usuários.

## 🎯 Objetivo
Simular o fluxo completo de um sistema de login seguro, aplicando bloqueio preventivo contra ataques de força bruta (tentativas repetidas de adivinhação de senha).

## ✨ Funcionalidades
- **Cadastro de Usuário:** Criação de conta com validação para impedir nomes de usuário duplicados e senhas vazias.
- **Autenticação Segura:** Verificação de credenciais no momento do login.
- **Controle de Tentativas:** O sistema monitora erros de senha.
- **Bloqueio de Conta:** Após 3 tentativas incorretas, o usuário é bloqueado e impedido de tentar novamente, simulando uma medida real de segurança.

## 🛠️ Tecnologias e Estruturas Utilizadas
- **Python 3.x**
- **Dicionários Aninhados:** Para armazenar de forma estruturada o estado de cada usuário `{"usuario": {"senha": str, "tentativas": int, "bloqueado": bool}}`.
- **Modularização (Funções):** Código dividido em funções específicas (`cadastrar_usuario`, `realizar_login`, `validar_senha`) para facilitar a manutenção e leitura.
- **Controle de Fluxo:** Uso intenso de `if/elif/else` para validações e loops `while` para manter a aplicação ativa.

## 🚀 Como Executar
1. Certifique-se de ter o Python instalado.
2. Clone este repositório ou baixe o arquivo `.py`.
3. Abra o terminal na pasta do arquivo e execute:
   ```bash
   python sistema_login.py

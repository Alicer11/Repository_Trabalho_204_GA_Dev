# Grupo_de_Testes-Back-End_204_G3

# 💻 Projeto Back-End — *Testes e Qualidade no Desenvolvimento*

> **Grupo Responsável**: G3 (Grupo_3)  
> **Função**: Criar, executar e documentar os testes do Back-End da aplicação.

---

## 🧠 O que é Back-End?

O **Back-End** é o cérebro da aplicação — a parte que **o usuário não vê**, mas que faz tudo acontecer por trás da interface. Ele lida com:

- 🔐 **Autenticação de usuários**
- 🛢️ **Acesso e manipulação de dados em bancos**
- 📡 **APIs para comunicação com o Front-End**
- ⚙️ **Lógica de negócios**

---

## 🧪 O que são Testes de Back-End?

**Testes de Back-End** verificam se o sistema está funcionando **corretamente, de forma segura e performática**. Eles garantem que o servidor, a base de dados e as APIs estejam de acordo com o que foi planejado.

### 🔍 Por que testar o Back-End?

✔️ Evita bugs e falhas de segurança  
✔️ Garante respostas corretas das APIs  
✔️ Confirma que os dados estão salvos e recuperados corretamente  
✔️ Aumenta a qualidade do sistema e a confiança da equipe  

---

## 🧰 Ferramentas Populares de Teste

| Ferramenta | Tipo de Teste | Descrição |
|-----------|----------------|-----------|
| 🧪 **Postman** | API | Teste manual e automatizado de APIs |
| 🧪 **Jest** | Unitário/Integração (JS) | Teste de funções e rotas em Node.js |
| 🧪 **Mocha + Chai** | Unitário/Integração (JS) | Testes flexíveis e assertions em Node.js |
| 🧪 **JUnit** | Java | Framework clássico para testes de Java |
| 🧪 **Docker** | Ambiente | Roda testes em ambientes isolados |

---

## 🧬 Tipos de Testes no Back-End

| Tipo | Descrição | Exemplo |
|------|-----------|---------|
| 🧪 **Teste Unitário** | Testa funções isoladas | Uma função que calcula frete |
| 🔗 **Teste de Integração** | Verifica integração entre módulos | API + Banco de Dados |
| 🚀 **Teste de Performance** | Mede velocidade e estabilidade | 1000 usuários simultâneos |
| 🛡️ **Teste de Segurança** | Detecta falhas e vulnerabilidades | Injeção de SQL |
| ♻️ **Teste de Regressão** | Verifica se nada foi quebrado após mudanças | Atualizou o sistema? Testa tudo de novo! |

---

## 🛠️ Como nosso grupo aplicará os testes

### 🎯 Etapas seguidas:

1. **Planejamento de Testes**  
   🔎 Identificamos os principais pontos críticos da aplicação: rotas da API, autenticação e banco de dados.

2. **Criação dos Casos de Teste**  
   📝 Usamos o Postman para simular requisições (GET, POST, PUT, DELETE) e o Jest para testar funções do sistema.

3. **Execução e Verificação**  
   ✅ Validamos status das respostas (200, 404, 500), tempo de resposta e integridade dos dados.

4. **Automatização com CI**  
   🤖 Integramos os testes ao GitHub Actions para rodarem automaticamente a cada commit.

5. **Relatórios de Resultados**  
   📊 Geramos logs e relatórios para o time de desenvolvimento analisar e corrigir erros.

---

## 🧾 Exemplo de Teste de API (Postman)

```json
GET /api/users/1

✔️ Esperado: status 200  
✔️ Corpo: 
{
  "id": 1,
  "nome": "João",
  "email": "joao@email.com"
}
Caso o ID não exista:
HTTP/1.1 404 Not Found

{
  "erro": "Usuário não encontrado"
}

# 🛡️ Teste de Phishing com SEToolkit – Formação Cybersecurity Specialist (DIO.me)

Este repositório documenta um exercício prático de **engenharia social** utilizando o **Social-Engineer Toolkit (SEToolkit)**, com o objetivo de simular um ataque de **phishing** e demonstrar a captura de credenciais em ambiente controlado. A atividade foi realizada como parte do curso de **Formação Cybersecurity Specialist** da plataforma [DIO.me](https://www.dio.me/).

---

## 🎯 Objetivo

Simular um ataque de phishing baseado em engenharia social, utilizando o SEToolkit, com o intuito de:

- Clonar uma página de login falsa;
- Observar o comportamento do usuário em uma interface conhecida;
- Capturar credenciais de forma controlada e ética para fins de estudo.

---

## 🛠️ Ferramentas Utilizadas

- 🐧 **Sistema Operacional:** Kali Linux (imagem oficial VirtualBox)
- 🧰 **Ferramenta:** SEToolkit (Social-Engineer Toolkit) – versão 8.x
- 🌐 **Técnica:** Credential Harvester + Web Templates

---

## 🚀 Etapas do Teste

### 1. Execução do SEToolkit

```bash
sudo setoolkit
```

Navegação nos menus:

```
> Social-Engineering Attacks
> Website Attack Vectors
> Credential Harvester Attack Method
> Web Templates
> Google
```

2. Geração do Site Falso
Inicialmente, foi tentada a clonagem da página do Facebook, mas o SEToolkit não conseguiu replicar a estrutura complexa do site devido a proteções modernas (JavaScript dinâmico, Content Security Policy, etc). Por isso, optou-se por usar o template falso do Google disponibilizado pelo SET.

A ferramenta iniciou automaticamente um servidor com a página falsa de login do Google, disponível no seguinte endereço de rede local:

```
http://192.168.0.109
```

### 3. Captura de Credenciais

Ao acessar a página e inserir dados de login, o terminal do SET exibiu os dados capturados:

```
[*] Username: navaia@dio.me
[*] Password: teste123
```

🔗 Prints e evidências disponíveis na pasta [`/images`](./images).

---

## 📸 Evidências

Imagens capturadas durante o teste:

- `tela-falsa-google.png`: página de login falsa criada pelo SET
- `terminal-credenciais.png`: exibição das credenciais no terminal

Acesse a pasta: [`/images`](./images)

---

## 📚 Lições Aprendidas

- Ferramentas como o SET são ótimas para fins didáticos, mas limitadas contra sites modernos.
- Sites como o Facebook dificultam clonagens com CSP, JavaScript dinâmico e autenticação reforçada.
- A atenção do usuário à **URL**, ao **HTTPS** e ao uso de **autenticação em dois fatores (2FA)** é essencial para evitar ataques de phishing.
- A **engenharia social** continua sendo um dos maiores riscos à segurança digital, muitas vezes mais eficaz que exploits técnicos.

---

## ✅ Conclusão

O teste foi concluído com sucesso, utilizando o **template do Google** incluso no SEToolkit. A simulação permitiu demonstrar como ataques de phishing funcionam na prática e reforçou a importância da **educação em segurança da informação** para prevenir esse tipo de ataque.

---

## ⚠️ Aviso Legal

> Este projeto tem **fins exclusivamente educacionais**. Nenhuma ação ofensiva real foi realizada contra terceiros.
>
> Utilizar técnicas de phishing fora de ambientes controlados e sem autorização é **crime** segundo a legislação brasileira (Lei nº 12.737/2012 – Lei Carolina Dieckmann).
>
> Sempre utilize seus conhecimentos de segurança de forma **ética e responsável**.

---

## 👤 Autor

- **Filipe L. Andrade**  
- Curso: Formação Cybersecurity Specialist – [DIO.me](https://www.dio.me/)

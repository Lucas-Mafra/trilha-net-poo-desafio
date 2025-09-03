# DIO - Trilha .NET - Programação Orientada a Objetos

Projeto desenvolvido como parte da trilha .NET da [DIO](https://www.dio.me/), focado em conceitos de Programação Orientada a Objetos (POO).

## Desafio

Modelar um sistema de celulares utilizando abstração, herança e polimorfismo. O objetivo é criar uma estrutura que permita diferentes marcas e modelos de smartphones terem comportamentos próprios, promovendo reuso de código.

## Contexto

Você é responsável por criar a abstração de um celular, permitindo que marcas como Nokia e iPhone implementem suas particularidades, especialmente no processo de instalação de aplicativos.

## Especificação

- **Classe Abstrata:** `Smartphone`
  - Não pode ser instanciada diretamente.
  - Serve como modelo para outras classes.
- **Classes Filhas:** `Nokia` e `Iphone`
  - Devem herdar de `Smartphone`.
  - Devem sobrescrever o método `InstalarAplicativo`, pois cada uma possui uma forma diferente de instalar aplicativos.

### Diagrama de Classes

![Diagrama classes](Imagens/diagrama.png)

## Estrutura do Projeto

```
trilha-net-poo-desafio/
│
├── Program.cs
├── Models/
│   ├── Smartphone.cs
│   ├── Nokia.cs
│   └── Iphone.cs
└── README.md
```

## Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/seu-repo.git
   cd trilha-net-poo-desafio
   ```

2. **Restaure e execute o projeto:**
   ```bash
   dotnet restore
   dotnet run
   ```

## Exemplo de Uso

Ao executar o projeto, você verá exemplos de criação de smartphones e instalação de aplicativos:

```
Smartphone Nokia:
Número: 11999999999
Modelo: Nokia 3310
IMEI: 123456789
Memória: 32
Instalando aplicativo WhatsApp no Nokia...

Smartphone iPhone:
Número: 11988888888
Modelo: iPhone 13
IMEI: 987654321
Memória: 128
Instalando aplicativo Instagram no iPhone...
```

## Regras e Validações

1. A classe **Smartphone** deve ser abstrata.
2. As classes **Nokia** e **Iphone** devem herdar de **Smartphone**.
3. O método **InstalarAplicativo** deve ser sobrescrito em ambas as classes filhas.

## Contribuição

Sinta-se à vontade para abrir issues ou pull requests para melhorias!

---
Projeto para fins educacionais.
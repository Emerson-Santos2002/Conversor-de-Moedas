<h1 align="center">Currency Converter</h1>

<p align="center">
  <a href="https://opensource.org/licenses/Apache-2.0"><img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/></a>
  <a href="https://android-arsenal.com/api?level=23"><img src="https://img.shields.io/badge/API-23%2B-brightgreen.svg?style=flat" border="0" alt="API"></a>
  <br>
  <a href="https://wa.me/+5571991154541"><img alt="WhatsApp" src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/emerson-dos-santos-silva-398319206/"><img alt="Linkedin" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:emersonsantos1921@gmail.com"><img alt="Gmail" src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
</p>

<p align="center">  

⭐ Esse é um projeto para demonstrar meu conhecimento técnico no desenvolvimento Android nativo com Kotlin. Mais informações técnicas abaixo.

Aplicativo que faz conversão de algumas moedas mais utilizadas com uma taxa de conversão recebida pela web, e com texto formatado com base nas moedas selecionadas.

</p>

</br>

<p float="left" align="center">
<img alt="screenshot" width="30%" src="screenshots/screenshot-1.png"/>
<img alt="screenshot" width="30%" src="screenshots/screenshot-2.png"/>
<img alt="screenshot" width="30%" src="screenshots/screenshot-3.png"/>
</p>

## Download
Faça o download da <a href="apk/app-debug.apk?raw=true">APK diretamente</a>. Você pode ver <a href="https://www.google.com/search?q=como+instalar+um+apk+no+android">aqui</a> como instalar uma APK no seu aparelho android. 

## Tecnologias usadas e bibliotecas de código aberto

- Minimum SDK level 23
- [Linguagem Kotlin](https://kotlinlang.org/)

- Jetpack -
  - Lifecycle: Observe os ciclos de vida do Android e manipule os estados da interface do usuário após as alterações do ciclo de vida.
  - LiveData: Notifica as estruturas de Views quando há alterações nas informações da ViewModel.
  - ViewModel: Gerencia o detentor de dados relacionados à interface do usuário e o ciclo de vida. Permite que os dados sobrevivam a alterações de configuração, como rotações de tela.
  - DataBinding: Vincula dados observáveis a elementos da interface do usuário em seu layout declarativamente atráves do binding.
  - Custom Views: View customizadas feitas do zero usando XML.

- Arquitetura - 
  - MVVM (View - ViewModel - Model)
  - Comunicação da ViewModel com a View através de LiveData.
  - Comunicação da ViewModel com a Model através do repositório que executa as requisições Web.
  - Repositories para abstração da comunidação com a camada de dados.
  
- Bibliotecas - 
  - [Retrofit2 & OkHttp3](https://github.com/square/retrofit): Para realizar requisições seguindo o padrão HTTP.
  - [Google/Gson](https://github.com/google/gson): Para realizar a conversão da requisição no formato Gson.

## Arquitetura
**Conversor De Moedas** utiliza a arquitetura MVVM, o padrão de Repositories e Singleton, que segue as [recomendações oficiais do Google](https://developer.android.com/topic/architecture).
</br></br>
<img alt="screenshot" width="60%" src="screenshots/arquitetura.png"/>
<br>

## API de terceiros

Conversor de moedas usa a Currency API do usuário do Github [fawazahmed0](https://github.com/fawazahmed0/currency-api) para suas chamadas REST.<br>
Esta API disponibiliza gratuitamente uma API REST completa de lista de moedas e suas taxas de conversão.

## Features

### Conversão de moedas
<img src="screenshots/feature-1.gif" width="25%"/>

Informação no topo sobre as moedas e taxa de conversão, seleção de moedas utilizando a Custom View Spinner.

### Inversão das moedas
<img src="screenshots/feature-2.gif" width="25%"/>

Formatação e Conversão de moedas de forma dinâmica com base na digitação do usuário utilizando Listeners e bibliotecas de formatação do java. Inversão das moedas através de um evento de clique.

# Licença

```xml
   Copyright [2023] [Emerson Dos Santos Silva]

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

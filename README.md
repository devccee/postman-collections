# Plataforma de Integração CCEE - Postman Collection

Conjunto de colections pré-configurados para serem rodados no [Postman](https://www.getpostman.com/) contém exemplos de chamadas dos serviços expostos pela [Plataforma de Integração CCEE](https://www.ccee.org.br/web/guest/documentos/plataforma-de-integracao).

## Utilização

Para utilizar esse Postman Collection, consider qualquer uma das opções abaixo:

* Acesse a documentação do Postman Collection que está disponível em https://documenter.getpostman.com/view/12351215/TVCdzTxD
* Acesse o arquivo em formato JSON que está salvo nesse repositório [Plataforma de Integração CCEE.postman_collection.json](Plataforma%20de%20Integração%20CCEE.postman_collection.json)
* Clique no botão abaixo e abra a configuração direto no Postman instalado em seu computador

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/27dc730daa9ea47cfa3e)

Para mais informações sobre o Postman, acesse https://www.postman.com/

## A Plataforma de Integração CCEE

A [Plataforma de Integração](https://www.ccee.org.br/web/guest/documentos/plataforma-de-integracao) é uma ferramenta que conecta os sistemas dos agentes com os sistemas da CCEE.

A solução complementa os canais de acesso oferecidos pela CCEE para conectar o negócio do cliente de forma simples e acessar informações com rapidez, segurança e confiabilidade.

Entre os benefícios para os agentes que utilizam a plataforma estão:
- Redução de atividades manuais por meio da integração entre sistemas
- Menor custo e risco operacional com a automatização de rotinas
- Maior agilidade e qualidade na integração e no intercâmbio de dados entre CCEE e demais participantes do mercado

## Quem pode utilizar

Agentes e consultorias que tenham representação total dos seus clientes aderidos à CCEE.

## Como aderir

Para utilizar a solução, basta possuir um certificado digital e realizar um cadastro na CCEE. Veja como é simples:
1. [Adquira um certificado digital](https://estrutura.iti.gov.br/)
2. [Cadastre-se na Plataforma de Integração da CCEE](https://www.ccee.org.br/documents/80415/919484/Ades%C3%A3o%20e%20Atualiza%C3%A7%C3%A3o%20Certificado%20e%20Senha%20Plataforma%20de%20Integra%C3%A7%C3%A3o%20no%20SGP_1.pdf/2cf3ef8e-16f5-2a17-9e7a-76abd25e1417)

## Como utilizar

Com o certificado instalado e o cadastro realizado, o próximo passo é conectar seu sistema aos serviços da plataforma. Veja abaixo como utilizar cada um deles.

## Primeiros passos

- [Guia de Primeiros Passos](https://github.com/devccee/guia-primeiros-passos)
- [Manual de Autenticação](https://www.ccee.org.br/documents/80415/919484/Autenticacao.pdf/5960714a-70e2-6c8d-9801-233fb34fb0fe)
- [Guia de medições](https://github.com/devccee/guia-medicoes)
- [Guia de contratos](https://www.ccee.org.br/documents/80415/919484/Manual%20servi%C3%A7os%20contratos.pdf/5a036b58-6e74-d2d5-acb3-d5fc8e96dc05)
- [Guia dos serviços de Webhook](https://github.com/devccee/webhook)
- [Guia dos serviços de acrônimos](https://www.ccee.org.br/documents/80415/919484/Manual%20servi%C3%A7os%20acr%C3%B4nimos%20DRI_v4.0.pdf/8ae1855c-83cf-16eb-fe0d-9cc6c207843d)
- [Manual de Alertas e exceções](https://www.ccee.org.br/documents/80415/919484/ManualDeExce%C3%A7%C3%B5es%20DaPlataformaDeIntegracao.pdf/9fe61c50-3cf6-7629-def2-94c94122f064)
- [Guia dos serviços de relatórios e resultados](https://www.ccee.org.br/documents/80415/919484/Manual%20servi%C3%A7os%20listar%20relat%C3%B3rios%20e%20resultados%20DRI_v3_0.pdf/135225de-e663-81fb-1c6a-2eeeba1cc5bf)
- [Guia dos serviços de PLD](https://www.ccee.org.br/documents/80415/919484/Manual%20usuario%20servi%C3%A7os%20listar%20PLD_v2.0.pdf/3f2784d9-c03d-1217-1f71-031a78f8f70c)

## Configurar autenticação SSL mútua no Postman

Um dos requisitos para autenticação nos serviços da Plataforma de Integração é a autenticação SSL mútua. Isso quer dizer que, ao acessar os web services da CCEE, será necessário utilizar uma chave privada de um certificado previamente cadastrado na Plataforma de Integração.

Os passos abaixo mostram como configurar sua chave privada no Postman:

1. Verique se tem acesso à sua chave privada, em arquivo no formato *.PFX, *.P12, *.JKS ou similar

2. No Postman, acesse _File > Settings_
![Postman - Howto 2Way SSL](./img/howto_postman_2wayssl_001.gif)

3. Adicione o arquivo com sua chave privada no campo _PFX File_, informando a senha do arquivo, e adicione o endereço o valor **_*.ccee.org.br_** no campo _Host_
![Postman - Howto 2Way SSL](./img/howto_postman_2wayssl_002.png)

## Referências

- [Postman Learning Center](https://learning.postman.com/)
- [Postman - Working with certificates](https://learning.postman.com/docs/sending-requests/certificates/)

------
_Agredecimentos_

* [Diego Yosiura](https://www.linkedin.com/in/diegoyosiura/), por compartilhar a ideia original de criar um Postman Collection para os serviços da Plataforma de Integração, bem como compartilhar atualizações em seu arquivo.

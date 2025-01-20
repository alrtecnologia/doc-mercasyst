# Habilitação do Serviço Scanntech no PDV Mercasyst

Este guia destina-se a auxiliar usuários a habilitarem o serviço da Scanntech no PDV Mercasyst, garantindo que as promoções sejam aplicadas corretamente e a comunicação com a plataforma funcione sem problemas.

## Requisitos Prévios

Antes de iniciar, certifique-se de que:

- O PDV Mercasyst esteja devidamente instalado e atualizado para a última versão.
- Você tenha uma conexão ativa com a internet.
- Um cadastro ativo na Scanntech com suas credenciais (CNPJ, e-mail, etc.).

## Passo a Passo para Habilitação

### 1. Cadastro na Scanntech

- Acesse a página de cadastro: [Clube de Promos - Cadastro](https://clubedepromos.com.br/#/contacto/minorista/).
- Preencha os seguintes dados no formulário:
    - **Nome completo**
    - **CNPJ** (obrigatório para empresas varejistas)
    - **E-mail** e **telefone** para contato
    - Dados adicionais solicitados (ex.: nome da rede varejista, endereço, etc.)
- Confirme seu cadastro e aguarde o contato da equipe da Scanntech para orientações sobre a ativação do serviço.

### 2. Configuração do Mercasyst

- **Acesse o Painel Administrativo do Mercasyst**:
    
    - No PDV, faça login com suas credenciais de administrador.
    - Navegue até a seção "Configurações > Integrações #3" e selecione a área "Parâmetros Scanntech".
- **Preencha os Parâmetros de Configuração**: De acordo com os dados exigidos na tela:
    
     - **Usuário**: Insira o e-mail do integrador fornecido pela Scanntech (ex.: `test@seu_email.com`).
    - **Senha**: Use a senha do integrador (ex.: `sua senha`).
    - **URL Base**: Insira a URL base da API da Scanntech, geralmente `http://br.homo.apipdv.scanntech.com/`.
    - **EndPoint Vendas**: Informe o endpoint para envio de dados de vendas (ex.: `movimientos`).
    - **EndPoint Promoções**: Informe o endpoint para sincronização de promoções (ex.: `promos`).
    - **EndPoint Fechamentos**: Informe o endpoint de fechamentos (ex.: `fecha`).
    - **ID Empresa**: Informe o ID fornecido pela Scanntech, como `83397`.
    - **ID Local**: Informe o identificador do local (ex.: `1`).
    - **Tempo de Sincronização (min)**: Configure o intervalo de tempo para sincronização automática de dados (ex.: `30` -> que é equivalente a 30 minutos).
    - **URL 2 e URL 3**: Certifique-se de que estejam iguais à URL Base, salvo orientação contrária da Scanntech.
    - **Data de Início**: Insira a data a partir da qual o serviço deve ser ativado (ex.: `22/04/2024`).
- **Salve as Configurações**:
    
    - para salvar não será necessário clique em botão de "salvar" pois os dados serão salvos progressivamente conforme for digitando os dados dos parâmetros.


##  3: Habilitação do Serviço

  ### Login no Serviço Scanntech

- Agora acessando o site oficial da Scanntech [aqui](https://clubedepromos.com.br/#/contacto/minorista/) vamos em entrar e faça login com os dados fornecidos pós cadastro na plataforma.
    
    

---

## 4: Aceitação de Promoções

### Acessando o Painel da Scanntech

- Após configurar o serviço no Mercasyst, acesse o painel de promoções [aqui](https://clubedepromos.com.br/#/contacto/minorista/)  e clicando em "Entrar" o usuário deve fazer login com suas credenciais.
    
- Navegue até a seção de promoções disponíveis, como mostrado na imagem abaixo:


<img width="1087" alt="Pasted image 20250118003630" src="https://github.com/user-attachments/assets/29effe49-b4b0-4eee-b0f2-c7e6496f65e9" />

    

### Interagindo com as Promoções

- **Filtrar Promoções**: Use os filtros disponíveis para visualizar promoções por status (Sem ação feita, Aceita, Rejeitada) ou por data.
    
- **Visualizar Promoções**:
    
    - Clique em uma promoção para ver detalhes como preço antigo, preço novo, desconto e validade.
        
- **Aceitar ou Rejeitar**:
    
    - Para aceitar uma promoção, clique em **Aceitar**.
        
    - Caso não seja interessante, clique em **Rejeitar**.
        
- **Observação de Preços**: Note a mensagem de alerta sobre preços acima do mercado, caso exibida.
    

### Ações em Lote

- Para aceitar várias promoções de uma vez, utilize a opção **Aceitar em Lote**.
    
-  Você também pode baixar a lista de promoções utilizando a opção **Baixar promoções**.
    

# Visualização de Promoções no PDV

- Ao acessar a dashboard de promoções Scanntech no pdv ele listará todas as promoções aceitas, rejeitadas, e promoções com problemas.
  
  - Uma promoção pode ter problemas quando ao ser aceita, os produtos elegíveis para a promoção ainda não esteja cadastrado no sistema, a dashboard no Mercasyst informara de maneira visual nos carde, orientando quais produtos devem ser cadastrado para que o erro seja corrigido. 

![Imagem do WhatsApp de 2025-01-16 à(s) 09 40 31_03177d0f](https://github.com/user-attachments/assets/c7d9cd97-ab5a-4bb5-abfc-b776d7a75f65)



---

## Conclusão

Após seguir os passos descritos, o serviço Scanntech estará habilitado no PDV Mercasyst e as promoções poderão ser gerenciadas diretamente pelo painel. Em caso de dúvidas, entre em contato com o suporte técnico da Scanntech ou de sua empresa para assistência adicional.

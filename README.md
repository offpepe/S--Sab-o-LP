# Só Sabão LP

### Propósito

Capitar email de clientes para uma proximidade maior, contato direto e estratégias de *mailing*

### Processo

Assim que a empresa passar o estatísticas de idade dos clientes será montada a aplicação embasado no público alvo da Só Sabão.

Com as estatísticas, será montado um protótipo *mobile-first*  de uma singlePage com design simples e de fácil habituação.

### Como será feito
A pagina iniciara com um carousel de noticias e informações em destaque da empresa, como por exemplo alguma data comemorativa da empresa ou alguma conquista recente, logo abaixo aparecerá a história da empresa, em seguida sua cultura, logo depois suas conquistas, seus produtos e por fim um formulário

Neste formulário terão os campos: nome, sobrenome, idade(opcional), email e telefone.

Estes dados serão utilizados para o contato, via email direto e whatsapp com chatbot ou consultor da loja.

A pagina será feita com **NextJS** por conta da sua simplicidade, para maior agilidade na sua montagem com o uso das funcionalidades server side, como por exemplo as *dinamyc api routes*, para a estilização será utilizado **CSS puro**, para garantir a identidade da empresa na página.

### Armazenamento

O armazenamento da página será feita via **MongoDB**, utilizando o serviço da Atlas, criando um Cluster na nuvem(DBaaS) com o MongoClient do módulo mongodb para a comunicação do back-end com o banco de dados.

Serão guardados os dados da seguinte forma:

    clients: [
	    {
		 name: 'John',
		 lastName: 'Doe',
		 age: 32,
		 email: 'john.doe@co.aktion.com',
		 tel: '+5564993425422',
	    },
    ]
obs: caso age não for preenchido deve ser cadastrada como `null`

### Deployment

A aplicação deve ser subida para produção utilizando algum PaaS com ampla possibilidade de configurar o container, como exemplo o **Heroku**.

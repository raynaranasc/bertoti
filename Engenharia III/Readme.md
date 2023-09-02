|nome do padrão|anti-padrão|definição do padrão|problema que ele resolve|Exemplo|
|---|---|---|---|---|
|Strategy |Herança|	encapsula uma familia de algoritmos usando composição e os torna intercambiaveis usando polimorfismo|Encapsulamento      |aplicativo de processamento de pagamentos que permite que os usuários escolham entre diferentes estratégias de pagamento, como cartão de crédito ou transferência bancária|
|Observer |Alto Acoplamento|Notificar objetos separados, em um mesmo evento/método|utilizamos o polimorfismo mas sem ocorrer o alto-acoplamento|aplicativo de previsão do tempo, onde várias partes do aplicativo precisam ser atualizadas quando há uma mudança nas condições meteorológicas|
|Composite|herança & alto-acoplamento|utilizamos o polimorfismo mas sem ocorrer o alto-acoplamento|Tratar objetos individuais e grupos de objetos de forma uniforme|uma estrutura hierárquica de arquivos e diretórios, onde um diretório pode conter subdiretórios e arquivos|

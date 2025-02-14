# Casos de testes para as DHT's

## 1 - Busca de um Valor Existente  
**Pré-requisito:** O par chave-valor já foi inserido na DHT.  
**Passos:**  
1. Solicitar a recuperação do valor associado a uma chave conhecida.  
2. Confirmar se o valor retornado corresponde à chave.  
**Resultado esperado:** O valor correto é retornado sem erros.  

## 2 - Atualização de um Valor Existente  
**Pré-requisito:** Um par chave-valor já foi inserido na DHT.  
**Passos:**  
1. Atualizar o valor associado a uma chave existente.  
2. Consultar a chave para verificar se o novo valor foi armazenado.  
**Resultado esperado:** O valor é atualizado corretamente e refletido na consulta. 

## 3 - Verificação de Desempenho com Grande Volume de Dados  
**Pré-requisito:** A DHT está ativa e possui nós suficientes para suportar um grande volume de dados.  
**Passos:**  
1. Inserir um grande número de pares chave-valor (exemplo: 1000 pares).  
2. Medir o tempo de inserção e recuperação.  
3. Verificar se a DHT mantém a consistência dos dados.  
**Resultado esperado:** A DHT lida com o grande volume de dados sem perda de desempenho ou consistência.

## 4 - Verificação de Chaves com Caracteres Especiais  
**Pré-requisito:** A DHT está ativa e possui pelo menos um nó em funcionamento.  
**Passos:**  
1. Inserir um par chave-valor onde a chave contém caracteres especiais (exemplo: O nome de um aluno que tem acento (Bárbara)).
2. Consultar a chave para verificar se a DHT lida corretamente com caracteres especiais.  
**Resultado esperado:** A DHT deve armazenar e recuperar chaves com caracteres especiais sem erros. 

## 5 - Verificação de Limite de Armazenamento  
**Pré-requisito:** A DHT está ativa e possui um limite de armazenamento definido.  
**Passos:**  
1. Inserir pares chave-valor até atingir o limite de armazenamento da DHT.  
2. Tentar inserir um novo par após o limite ser atingido.  
3. Verificar como a DHT lida com o excesso de dados (exemplo: rejeição ou substituição).  
**Resultado esperado:** A DHT deve tratar o limite de armazenamento de forma consistente, sem corromper dados existentes. 

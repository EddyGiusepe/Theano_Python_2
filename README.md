'''
Data Scientist Jr.: Dr.Eddy Giusepe Chirinos Isidro
'''

# Lesson06: Usando os modelos Keras com o Scikit-Learn
A biblioteca ``scikit-learn`` é uma estrutura de aprendizado de máquina de propósito geral em 
Python desenvolvida com base no ``SciPy``. O ``Scikit-learn`` se destaca em tarefas como avaliar
o desempenho do modelo e otimizar os hiperparâmetros do modelo em apenas algumas linhas de código.

``Keras`` oferece uma classe de wrapper que permite que você use seus modelos de aprendizado profundo
com o scikit-learn. <font color="orange">Por exemplo</font>, uma instância da classe 
<font color="orange">KerasClassifier</font> em Keras pode envolver seu modelo de aprendizado
profundo e ser usada como um Estimador no ``scikit-learn``. Ao usar a classe
<font color="orange">KerasClassifier</font>, você deve especificar o nome de uma função que a
classe pode usar para definir e compilar seu modelo. Você também pode passar parâmetros adicionais
para o construtor da classe KerasClassifier que serão passados para a chamada posteriormente
``model.fit()``, como o <font color="yellow">número de épocas</font> e o tamanho do lote
(<font color="yellow">batch size</font>).


Nesta lição, nosso objetivo é desenvolver um modelo de aprendizado profundo e avaliá-lo usando
a <font color="orange">validação cruzada</font> ``k-fold``.
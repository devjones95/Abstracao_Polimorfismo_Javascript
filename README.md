Abstração e Polimorfismo

Esse código ilustra **abstração** e **polimorfismo** na Programação Orientada a Objetos (POO).

1. **Abstração**: A classe base `Imovel` define um método abstrato `descrever()`, que não tem implementação na classe base, mas é esperado que seja implementado nas subclasses. Isso oculta a complexidade de como cada tipo de imóvel é descrito, permitindo que as subclasses forneçam a implementação específica. Ou seja, o comportamento de descrição de um imóvel é abstraído e deixado para as subclasses.

2. **Polimorfismo**: As classes `Casa` e `Apartamento` herdam de `Imovel` e implementam o método `descrever()`. Embora ambas implementem o mesmo método (`descrever`), o comportamento é diferente para cada classe. Quando chamamos `descreverImovel(imovel)`, o JavaScript executa a versão correta do método `descrever()` dependendo do tipo de objeto passado (se é uma `Casa` ou um `Apartamento`). Isso é o polimorfismo: o mesmo método tem comportamentos diferentes para diferentes tipos de objetos. 

Portanto, a função `descreverImovel()` pode manipular tanto `Casa` quanto `Apartamento`, sem precisar saber as diferenças internas de cada classe.

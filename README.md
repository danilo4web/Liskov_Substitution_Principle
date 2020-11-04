# Liskov_Substitution_Principle
LSP— Liskov Substitution Principle

```
<?php

#LSP— Liskov Substitution Principle

class A 
{
    public function getNome()
    {
        echo 'Meu nome é A';
    }
}

class B extends A 
{ 
    public function getNome()
    {
        echo 'Meu nome é B';
    }
}

$objeto1 = new A;
$objeto2 = new B;

function imprimeNome(A $objeto)
{
    return $objeto->getNome();
}

imprimeNome($objeto1); // Meu nome é A
imprimeNome($objeto2); // Meu nome é B
```

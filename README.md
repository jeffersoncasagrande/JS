# javascript
 class  Cliente {
    nome ;
    cpf ;
}

classe  ContaCorrente {
    agencia ;
     // #saldo = 0 https://github.com/tc39/proposal-class-fields#private-fields
    _saldo  =  0 ;

    sacar ( valor ) {
        if ( this . _saldo  > =  valor ) {
            isso . _saldo  - =  valor ;
             valor de retorno ;
        }
    }

    depositar ( valor ) {
        if ( valor  <=  0 )
        {
            retorno ;
        } 
        isso . _saldo  + =  valor ;           
    }
}

const  cliente1  =  novo  Cliente ( ) ;
cliente1 . nome  =  "Ricardo" ;
cliente1 . cpf  =  11122233309 ;

const  cliente2  =  novo  Cliente ( ) ;
cliente2 . nome  =  "Alice" ;
cliente2 . cpf  =  88822233309 ;


const  contaCorrenteRicardo  =  novo  ContaCorrente ( ) ;
contaCorrenteRicardo . agencia  =  1001 ;

contaCorrenteRicardo . depositar ( - 100 ) ;
contaCorrenteRicardo . depositar ( 100 ) ;
contaCorrenteRicardo . depositar ( 100 ) ;

const  valorSacado  =  contaCorrenteRicardo . sacar ( 50 ) ;
console . log ( valorSacado ) ;

console . log ( contaCorrenteRicardo ) ;


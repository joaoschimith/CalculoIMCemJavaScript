# CalculoIMCemJavaScript
Se você estiver nesse problema em seu curso/faculdade, este código irá lhe ajudar!

      function calcular(){
    		// pegando o id do formulario
    		var formulario = document.getElementById("formulario");	
    		
    		// kilos é minha variavel
    		// formulario é o id do meu formulario
    		// value é o valor do input
    		// o + na frente transforma em number a string	
    			
    		var kilos  		= +formulario.kilos.value;
    		var metros 		= +formulario.metros.value;
    		var centimetros = +formulario.centimetros.value;
    		
     		// altura
    		var altura = (metros * 100 + centimetros) / 100;
    		 
    		// imc
    		var imc = kilos / (altura * altura);
    		
    		// o metodo toFixed fixa apenas duas casas decimais apos o ponto.
    		formulario.imc.value = imc.toFixed(2);
    		
    		if(16 <= imc 16.9)
    		{
    			alert('Muito abaixo do peso');
    		} 
    		else if(17 <= imc 18.4)
    		{
    			alert("Abaixo do peso");
    		}
    		else if(imc >25 && imc <= 30)
    		{
    			alert("Peso normal");
    		}
    		else if(imc >30 && imc <= 35)
    		{
    			alert("Obesidade grau I");
    		}
    		else if(imc >35 && imc <= 40)
    		{
    			alert("Obesidade grau II");
    		}
    		else if(imc >40 && imc <= 50)
    		{
    			alert("Obesidade grau III");
    		}
    		else
    		{
    			alert('Inválido');
    		}
    	}

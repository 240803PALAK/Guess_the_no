# Guess_the_no

Get detail of Phone Number like Timezone , Carrier, Register.


    <!DOCTYPE html>
    <html>
    <head>
    	<meta charset="utf-8">
    	<title>Number Guessing Game</title>
    
    	<style>
    		body {
    			font-family: sans-serif;
    			width: 50%;
    			max-width: 800px;
    			min-width: 480px;
    			margin: 0 auto;
    		}
    	</style>
    </head>
    
    <body>
    	<h1>Guess The Number</h1>
    	<p>
    		We have selected a random number 
    		between 1 - 10. See if you can
    		guess it.
    	</p>
    
    	<div class="form">
    		<label for="guessField">
    			Enter a guess: 
    		</label>
    		
    		<input type="text" id="guessField"
    			class="guessField">
    		
    		<input type="submit" value="Submit guess"
    			class="guessSubmit" id="submitguess">
    	</div>
    
    	<script type="text/javascript">
    
    		let y = Math.floor(Math.random() * 10 + 1);
    
    		let guess = 1;
    
    		document.getElementById("submitguess").onclick = function () {
    
    			let x = document.getElementById("guessField").value;
    
    			if (x == y) {
    				alert("CONGRATULATIONS!!! YOU GUESSED IT RIGHT IN "
    					+ guess + " GUESS ");
    			}
    
    			else if (x > y) {
    				guess++;
    				alert("OOPS SORRY!! TRY A SMALLER NUMBER");
    			}
    			else {
    				guess++;
    				alert("OOPS SORRY!! TRY A GREATER NUMBER")
    			}
    		}
    	</script>
    </body>
    </html>

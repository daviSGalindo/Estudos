(function () {
    const app = document.getElementById('app');
  
    app.innerHTML = `
      <div class="container">
        <h1>Validador de Telefone</h1>
        <input type="text" id="telefone" placeholder="Digite o número de telefone">
        <div id="resultado" class="card"></div>
      </div>
    `;
  
    function validarTelefone(numero) {
      const padrao = /^(\+55\s?)?(\(?\d{2}\)?\s?)?9\d{4}-?\d{4}$/;
      return padrao.test(numero);
    }
  
    const inputTelefone = document.getElementById('telefone');
    const resultado = document.getElementById('resultado');
  
    inputTelefone.addEventListener('blur', () => {
      const numero = inputTelefone.value.trim();
      if (numero) {
        if (validarTelefone(numero)) {
          resultado.textContent = 'Número válido!';
          resultado.className = 'card valid';
          resultado.style.display = 'block';
        } else {
          resultado.textContent = 'Número inválido!';
          resultado.className = 'card invalid';
          resultado.style.display = 'block';
        }
      } else {
        resultado.textContent = '';
        resultado.style.display = 'none';
      }
    });
  })();
  

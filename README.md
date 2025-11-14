// Criando o objeto livro
let livro = {
    titulo: "Dom Casmurro",
    autor: "Machado de Assis",
    paginas: 256,
    disponivel: true
};

console.log(livro.titulo);
console.log(livro["autor"]);

livro.editora = "Editora XYZ";

livro.detalhes = function() {
    return `O livro "${this.titulo}", de ${this.autor}, possui ${this.paginas} páginas e é publicado pela ${this.editora}.`;
};

console.log(livro.detalhes());

let biblioteca = {
    livros: [livro]
};

// Funções
function saudar(nome) {
    return `Olá, ${nome}!`;
}

function calcularMedia(a, b, c) {
    return (a + b + c) / 3;
}

function apresentarProduto(nome, preco = 0) {
    return `Produto: ${nome} | Preço: R$ ${preco}`;
}

console.log(saudar("Gabriel"));
console.log(calcularMedia(9, 8, 10));
console.log(apresentarProduto("Mouse", 59.90));

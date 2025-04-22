-- Criação das tabelas
CREATE TABLE produtos (
    id INTEGER PRIMARY KEY,
    nome TEXT NOT NULL,
    preco DECIMAL(10,2),
    estoque INTEGER
);

CREATE TABLE pedidos (
    id INTEGER PRIMARY KEY,
    data DATE,
    produto_id INTEGER,
    quantidade INTEGER,
    FOREIGN KEY (produto_id) REFERENCES produtos(id)
);

-- Inserção de registros
INSERT INTO produtos (id, nome, preco, estoque) VALUES
(1, 'Livro A', 49.90, 10),
(2, 'Livro B', 79.90, 5),
(3, 'Livro C', 39.90, 8);

INSERT INTO pedidos (id, data, produto_id, quantidade) VALUES
(1, '2025-04-21', 1, 2),
(2, '2025-04-22', 2, 1),
(3, '2025-04-22', 3, 3);

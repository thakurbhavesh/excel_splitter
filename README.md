CREATE DATABASE excel_splitter;

USE excel_splitter;

CREATE TABLE files (
    id INT AUTO_INCREMENT PRIMARY KEY,
    file_name VARCHAR(255) NOT NULL,
    file_path VARCHAR(255) NOT NULL,
    file_type ENUM('parent', 'split') NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

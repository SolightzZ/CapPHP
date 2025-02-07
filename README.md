CREATE TABLE CatBreeds (
    id INT AUTO_INCREMENT PRIMARY KEY, 
    name_th VARCHAR(255) NOT NULL, 
    name_en VARCHAR(255) NOT NULL, 
    description TEXT NOT NULL, 
    characteristics TEXT, 
    care_instructions TEXT, 
    image_url VARCHAR(2083), 
    is_visible TINYINT(1) NOT NULL DEFAULT 1
);

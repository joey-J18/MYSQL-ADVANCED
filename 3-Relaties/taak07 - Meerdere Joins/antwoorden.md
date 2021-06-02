# Antwoorden

1. SELECT game.name, platform.platform, genre.genre FROM game LEFT JOIN platform ON game.platform_id = platform.id LEFT JOIN genre ON game.genre_id = genre.id WHERE game.name LIKE "b%";

2. SELECT game.name, platform.platform, genre.genre, publisher.publisher,game.year FROM game LEFT JOIN platform ON game.platform_id = platform.id LEFT JOIN genre ON game.genre_id = genre.id LEFT JOIN publisher ON game.platform_id = publisher.id WHERE game.year =2013;

3. SELECT game.name, game.year,game.global_sales, platform.platform, genre.genre FROM game LEFT JOIN platform ON game.platform_id = platform.id LEFT JOIN genre ON game.genre_id = genre.id WHERE game.global_sales AND game.year >2000;

4. SELECT game.name, game.year,game.jp_sales, platform.platform, genre.genre FROM game LEFT JOIN platform ON game.platform_id = platform.id LEFT JOIN genre ON game.genre_id = genre.id WHERE game.name LIKE "Mario%";

5. SELECT game.name, platform.platform, genre.genre, publisher.publisher,game.year FROM game LEFT JOIN platform ON game.platform_id = platform.id LEFT JOIN genre ON game.genre_id = genre.id LEFT JOIN publisher ON game.platform_id = publisher.id WHERE platform="PC";
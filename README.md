<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Random Recipe Generator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            text-align: center;
            width: 90%;
            max-width: 600px;
        }

        h1 {
            margin-bottom: 20px;
            font-size: 28px;
            color: #ff6f61;
        }

        .ingredients {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            margin-bottom: 20px;
        }

        label {
            background: #ff6f61;
            color: white;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.2s;
        }

        label:hover {
            transform: scale(1.05);
        }

        label input {
            margin-right: 5px;
            display: none;
        }

        button {
            background: #e55b50;
            color: white;
            border: none;
            padding: 10px 30px;
            border-radius: 30px;
            cursor: pointer;
            font-size: 18px;
            transition: background 0.3s;
        }

        button:hover {
            background: #ff6f61;
        }

        .recipe-container {
            margin-top: 30px;
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .recipe-container h2 {
            margin-bottom: 20px;
            font-size: 24px;
            color: #ff6f61;
        }

        .recipe-container pre {
            background: #f8f8f8;
            padding: 20px;
            border-radius: 10px;
            text-align: left;
            white-space: pre-wrap;
            font-size: 16px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .recipe-image {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Advanced Random Recipe Generator</h1>
        <form id="ingredientForm">
            <div class="ingredients">
                <label>
                    <input type="checkbox" name="ingredient" value="chicken"> Chicken
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="beef"> Beef
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="pasta"> Pasta
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="rice"> Rice
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="vegetables"> Vegetables
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="cheese"> Cheese
                </label>
            </div>
            <button type="button" id="generateRecipe">Generate Recipe</button>
        </form>
        <div id="recipeContainer" class="recipe-container"></div>
    </div>
    <script>
        const recipes = [
            {
                ingredients: ["chicken", "vegetables"],
                name: "Grilled Chicken with Vegetables",
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced Random Recipe Generator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #ffecd2 0%, #fcb69f 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            text-align: center;
            width: 90%;
            max-width: 600px;
        }

        h1 {
            margin-bottom: 20px;
            font-size: 28px;
            color: #ff6f61;
        }

        .ingredients {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
            margin-bottom: 20px;
        }

        label {
            background: #ff6f61;
            color: white;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            transition: transform 0.2s;
        }

        label:hover {
            transform: scale(1.05);
        }

        label input {
            margin-right: 5px;
            display: none;
        }

        button {
            background: #e55b50;
            color: white;
            border: none;
            padding: 10px 30px;
            border-radius: 30px;
            cursor: pointer;
            font-size: 18px;
            transition: background 0.3s;
        }

        button:hover {
            background: #ff6f61;
        }

        .recipe-container {
            margin-top: 30px;
            animation: fadeIn 1s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .recipe-container h2 {
            margin-bottom: 20px;
            font-size: 24px;
            color: #ff6f61;
        }

        .recipe-container pre {
            background: #f8f8f8;
            padding: 20px;
            border-radius: 10px;
            text-align: left;
            white-space: pre-wrap;
            font-size: 16px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .recipe-image {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Advanced Random Recipe Generator</h1>
        <form id="ingredientForm">
            <div class="ingredients">
                <label>
                    <input type="checkbox" name="ingredient" value="chicken"> Chicken
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="beef"> Beef
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="pasta"> Pasta
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="rice"> Rice
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="vegetables"> Vegetables
                </label>
                <label>
                    <input type="checkbox" name="ingredient" value="cheese"> Cheese
                </label>
            </div>
            <button type="button" id="generateRecipe">Generate Recipe</button>
        </form>
        <div id="recipeContainer" class="recipe-container"></div>
    </div>
    <script>
        const recipes = [
            {
                ingredients: ["chicken", "vegetables"],
                name: "Grilled Chicken with Vegetables",
                instructions: "1. Marinate the chicken.\n2. Grill the chicken.\n3. Sauté the vegetables.\n4. Serve together.",
                image: "https://photos.app.goo.gl/MSQevQkpym2NWGU58"
            },
            {
                ingredients: ["beef", "rice"],
                name: "Beef Stir-Fry with Rice",
                instructions: "1. Cook the rice.\n2. Stir-fry the beef.\n3. Mix with rice and vegetables.\n4. Serve hot.",
                image: "https://photos.app.goo.gl/oeQUAcKhsD5ePw9X7"
            },
            {
                ingredients: ["pasta", "cheese"],
                name: "Cheesy Pasta",
                instructions: "1. Boil the pasta.\n2. Prepare the cheese sauce.\n3. Mix pasta with sauce.\n4. Serve warm.",
                image: "https://photos.app.goo.gl/CYnm5Xhf7JHiNSxh6"
            }
        ];

        document.getElementById('generateRecipe').addEventListener('click', () => {
            const selectedIngredients = Array.from(document.querySelectorAll('input[name="ingredient"]:checked')).map(input => input.value);
            const filteredRecipes = recipes.filter(recipe => selectedIngredients.every(ing => recipe.ingredients.includes(ing)));

            const recipeContainer = document.getElementById('recipeContainer');
            recipeContainer.innerHTML = '';

            if (filteredRecipes.length > 0) {
                const randomRecipe = filteredRecipes[Math.floor(Math.random() * filteredRecipes.length)];
                const recipeElement = document.createElement('div');
                recipeElement.innerHTML = `
                    <h2>${randomRecipe.name}</h2>
                    <img src="${randomRecipe.image}" alt="${randomRecipe.name}" class="recipe-image">
                    <pre>${randomRecipe.instructions}</pre>
                `;
                recipeContainer.appendChild(recipeElement);
            } else {
                recipeContainer.innerHTML = '<p>No recipes found with the selected ingredients.</p>';
            }
        });
    </script>
</body>
</html>￼Enter                instructions: "1. Marinate the chicken.\n2. Grill the chicken.\n3. Sauté the vegetables.\n4. Serve together.",
                image: "https://photos.app.goo.gl/MSQevQkpym2NWGU58"
            },
            {
                ingredients: ["beef", "rice"],
                name: "Beef Stir-Fry with Rice",
                instructions: "1. Cook the rice.\n2. Stir-fry the beef.\n3. Mix with rice and vegetables.\n4. Serve hot.",
                image: "https://photos.app.goo.gl/oeQUAcKhsD5ePw9X7"
            },
      {
                ingredients: ["pasta", "cheese"],
                name: "Cheesy Pasta",
                instructions: "1. Boil the pasta.\n2. Prepare the cheese sauce.\n3. Mix pasta with sauce.\n4. Serve warm.",
                image: "https://photos.app.goo.gl/CYnm5Xhf7JHiNSxh6"
            }
        ];

        document.getElementById('generateRecipe').addEventListener('click', () => {
            const selectedIngredients = Array.from(document.querySelectorAll('input[name="ingredient"]:checked')).map(input => input.value);
            const filteredRecipes = recipes.filter(recipe => selectedIngredients.every(ing => recipe.ingredients.includes(ing)));

            const recipeContainer = document.getElementById('recipeContainer');

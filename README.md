<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Responsive Table</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <style>  
        /* Hide the table rows on small screens and show them as list items instead */  
        @media (max-width: 640px) {  
            .table {  
                display: none;  
            }  
            .list {  
                display: block;  
            }  
        }  
    </style>  
</head>  
<body class="bg-gray-100 p-6">  
    <div class="container mx-auto">  
        <h1 class="text-center text-2xl font-bold mb-4 underline hover:cursor-pointer"></h1>  
        
        <table class="table w-full border-collapse">  
            <thead>  
                <tr class="hover:bg-orange-500 text-white bg-green-500 hover:cursor-pointer">  
                    <th class="hidden sm:table-cell py-2 px-4 border">FIRST NAME</th>  
                    <th class="hidden sm:table-cell py-2 px-4 border">LAST NAME</th>  
                    <th class="hidden sm:table-cell py-2 px-4 border">AGE</th>  
                </tr>  
            </thead>  
            <tbody>  
                <tr class="hover:uppercase hover:underline bg-red-500 hover:cursor-pointer">  
                    <td class="py-2 px-4 border">Accrea</td>  
                    <td class="py-2 px-4 border">Fantasy</td>  
                    <td class="py-2 px-4 border">20</td>  
                </tr>  
                <tr class="hover:uppercase hover:underline bg-red-500 hover:cursor-pointer">  
                    <td class="py-2 px-4 border">Hess</td>  
                    <td class="py-2 px-4 border">Ceana</td>  
                    <td class="py-2 px-4 border">19</td>  
                </tr>  
            </tbody>  
        </table>  

        <div class="list hidden sm:block mt-4">  
            <div class="bg-orange-500 shadow-md rounded-lg p-4">  
                <div class="hover:cursor-pointer flex justify-between mb-3">  
                    <span class="font-bold underline">FIRST NAME:</span>  
                    <span class="hover:underline">Accrea</span>  
                </div>  
                <div class="hover:cursor-pointer flex justify-between mb-3">  
                    <span class="font-bold underline">LAST NAME:</span>  
                    <span class="hover:underline">Fantasy</span>  
                </div>  
                <div class="hover:cursor-pointer flex justify-between mb-3">  
                    <span class="font-bold underline">AGE:</span>  
                    <span class="hover:underline">20</span>  
                </div>  
            </div>  

            <div class="bg-orange-500 shadow-md rounded-lg p-4 mt-2">  
                <div class="hover:cursor-pointer flex justify-between mb-2">  
                    <span class="font-bold underline">FIRST NAME:</span>  
                    <span class="hover:underline">Hess</span>  
                </div>  
                <div class="hover:cursor-pointer flex justify-between mb-2">  
                    <span class="font-bold underline">LAST NAME:</span>  
                    <span class="hover:underline">Ceana</span>  
                </div>  
                <div class="hover:cursor-pointer flex justify-between mb-2">  
                    <span class="font-bold underline">AGE:</span>  
                    <span class="hover:underline">19</span>  
                </div>  
            </div>  
        </div>  
    </div>  
</body>  
</html>

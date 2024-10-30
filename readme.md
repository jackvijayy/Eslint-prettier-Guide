
<div align="center">

![5](https://github.com/user-attachments/assets/c54fead2-a3d7-4006-bbae-575e145c6b62)

#  <a name="table">TABLE OF CONTENT </a>

</div>




1. 🤖 [Introduction](#introduction)

2. ⚙️ [Next js setup](#nextjs-setup)
 
3. ⚙️️[React js setup](#reactjs-setup)
4. 🤸 [Extension](#extention)




# <a name="introduction">🤖 Introduction</a>


## Introduction to Linting :

ESLint, and Prettier
Linting is the process of analyzing code for potential errors,
bugs, and stylistic issues. It helps maintain a consistent
code style, improves code quality, and catches common
mistakes early in development. Two popular tools for linting
modern web development code are ESLint and Prettier.


## What is Prettier?
Prettier is a code formatter that focuses on code
formatting and style consistency. It automatically formats
your code according to predefined rules, making it more
readable and eliminating debates over code style.
A code formatter is primarily concerned with the visual
appearance and consistent code formatting. It
automatically analyzes the structure of the code and
applies predefined formatting rules to ensure a uniform
style throughout the codebase.
Code formatters focus on aspects such as indentation, line
breaks, spacing, & the placement of braces & parentheses


## What is ESLint?
ESLint is a linter that allows you to define custom linting
rules and enforce coding standards. It helps identify and fix
potential errors, enforces consistent coding styles, and
promotes best practices in your codebase.
A code linter goes beyond code formatting and focuses on
the correctness, quality, and potential issues within the
code. Linters analyze the code for potential errors, bugs,
stylistic inconsistencies, and violations of coding standards
and best practices.
They check for issues such as unused variables, missing
semicolons, incorrect function usage, possible memory
leaks, and adherence to coding conventions.




 # <a name="nextjs-setup">⚙️ Next js setup</a>
 
 </br>
 
<div align="center">
<img src="https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" width=400 height=100 ></img >
</div>

# Next.js 14 Setup


Create Next.js Project using,

```base
npx create-next-app@latest

```


# Add an ESLint Config


If you look at the file at the root of your
new Next.js project, you’ll see that there is already an ESLint
configuration called next/core-web-vitals and standard.
It’s important to keep it. It will warn you when you write
code in your Next.js project that affects core web vitals.

 ### .eslintrc.json

We still need to add another ESLint configuration for
consistent code styling, as the default Next configuration
doesn’t do much to help you improve the quality of your
codebase.

Let’s install the standard configuration. Here are its . [rules](https://standardjs.com/rules.html)


Now, run:

```base
npm eslint-config-standard install

```

## Add an ESLint Config

https://jsmastery.pro JavaScript Mastery
This will install the standard ESLint configuration in your
project. Then, add it to your file: .eslintrc.json

```base
{
    "extends:["next/core-web-vitals","standard"]
}
```


## Testing ESLint in the Terminal

https://jsmastery.pro JavaScript Mastery
Now that we have added a new ESLint configuration let’s
run it with

```base
npm lint run

```

# Adding an ESLint Configuration for TailwindCSS

Having our class names organized logically in Tailwind
makes the code easier to read and review. We can install
another ESLint config that takes care of that to do this
automatically.

```base
npm eslint-plugin-tailwindcss install
```

and add it to your .eslintrc.json file like this:


```base
{
    "extends:["next/core-web-vitals","standard"],
    "plugin:tailwindcss/recommended"]
}
```

# Prettier VS ESLint potential conflicts

ESLint sometimes likes to enter into conflict with Prettier.

To avoid these situations, you should run:





```base
npm eslint-config-prettier install
```

This will install a package that removes all ESLint rules that
could conflict with Prettier. Once installed, add “prettier” to
your .eslintrc.json file.


```base
{
    "extends:["next/core-web-vitals","standard"],
    "plugin:tailwindcss/recommended","prettier"]
}
```






# Install Prettier

```base
npm prettier install

```


# Setting things up for VSCode

Now that everything is set up command-line-wise, it’s time
to integrate ESLint and Prettier with VSCode. For that, we will
need to modify the settings.json file or create a config
specific to our project that you can share with others if
you’d like. We’ll go with the latter.
In your Next.js project at the root, create a .vscode folder
and within it a settings.json file with the following code:

 
 # <a name="extension">Extension</a>
# Install ESLint and Prettier from the Extensions Marketplace

![Screenshot 2024-10-30 122954](https://github.com/user-attachments/assets/6b76fbbb-e907-4a4d-8045-9c01aa4d1101)

![Screenshot 2024-10-30 123022](https://github.com/user-attachments/assets/4dc8d514-57b4-46f6-ba7d-024da1af947c)



</br>

### IMPORTANT: Install the Prettier Eslint Package too (a third one!).

![Screenshot 2024-10-30 123202](https://github.com/user-attachments/assets/98730ddf-0388-489f-820d-09524b819801)

</br>

## Conclusion

You can finally start working on your project rather than
pulling your hair out with configurations.







 # <a name="#reactjs-setup">⚙️ React js setup</a>
 
 </br>
 
<div align="center">
<img src="https://shields.io/badge/react-black?logo=react&style=for-the-badge" width=400 height=100 ></img >
</div>

# 


Create react.js Project using,

```base
npm create vite@latest

```

Select React and TypeScript when asked.
Go inside created project, run install packages. Finally,
open the project in VSCode. By default ESLint is included in
the Vite project so you don’t have to reinstall ESLint.


Go inside created project, run install packages. Finally,
open the project in VSCode. By default ESLint is included in
the Vite project so you don’t have to reinstall ESLint.

```base
cd project_name
npm install

```
Finally, open the project in VSCode. By default ESLint is
included in the Vite project so you don’t have to reinstall
ESLint.




## React.js Setup


Remove the .eslintrc.cjs file at the root of the
project and replace it with a .eslintrc.json file with
the following content:

## React.js Setup

Install the required packages

```base
npm eslint-config-standard eslint-plugin-
tailwindcss eslint-config-prettier

```






* eslint-config-standard is a package for enforcingthe standard coding style.
 * eslint-plugin-tailwindcss is a package for enforcing logical ordering of Tailwind CSS classes.
 * eslint-config-prettier is a package to avoid conflicts between ESLint and Prettier.


### Install prettier package


```
npm prettier install

```


<div  align="center">

# The End 👀


# Congratulations on reaching the end of our guide! But hey,learning doesn't have to stop here.



</div>












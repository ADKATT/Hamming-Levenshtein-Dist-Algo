## About

With the help of this application you can calculate the Hamming distance (substitution values only) and Levenshtein distance of the given strings.

## Screenshots

__User Interface to calculate distance from Browser__
![Home Page](https://i.imgur.com/3rcpXTz.png)

__Input Field Validation Error:__
![Home Page with form error](https://i.imgur.com/djgifCX.png)

__Response__
![Home Page with response](https://i.imgur.com/aPQmXtn.png)

## Installation
Here is how you can run the project locally:
1.  Clone this repo
	```sh
	 git clone {REPOSITORY_URL}
	```
2.  Go into the project root directory
    ```sh
	 cd /distance-calculator
	```
3.  Copy `.env.example` file to `.env` file
    ```sh
	 cp .env.example .env
	```
4. Run the following command to install the dependency
	```sh
	 composer install
	```
5. Run the command to serve the project
	```sh
	 php artisan serve
	```
6. Open this link in your browser http://127.0.0.1:8000

## Run Calculation Using CLI

1. Goto your project directory using the following command.
	```sh
	 cd ./distance-calculator
	```
2. Run this command
	```sh
	 php artisan app:calculate
	```
3. Input first string and hit enter.
4. Input second string and hit enter.
5. You should see the distance calculation of both the strings in the result.

![CLI Output](https://i.imgur.com/sOB6U1C.png)

## Unit Tests

1. Goto the project directory using the following command.
	```sh
	 cd ./distance-calculator
	```
2. Run this command
	```sh
	 php artisan test
	```
![Unit Test](https://i.imgur.com/kR86isS.png)

## Folder Structure

*We are using the following files in this project.*

- __Controllers__
	- `App\Http\Controllers\IndexController.php`
- __Validation Requests__
	- `App\Http\Requests\Index.php`
- __Routes__
	- `Routes\Web.php`
- __View Templates__
	- `Resources\Views\layouts\app.blade.php`
	- `Resources\Views\index.blade.php`
- __Console Commands__
	- `App\Console\Commands\CalculationCommand.php`
- __Test Cases__
	- `Tests\Feature\IndexControllerTest.php`
	- `Tests\Unit\CalculationTest.php`

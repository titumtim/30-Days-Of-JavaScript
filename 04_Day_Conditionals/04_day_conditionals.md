Exercise: Level 2
1. let score = 80;
    if (score >= 80 && score <= 100) {
        cosole.log ('A');
    } else if (score >= 70 && score <= 79) {
        cosole.log ('B');
    } else if (score >= 60 && score <= 69) {
       cosole.log ('C');
    } else if (score >= 50 && score <= 59) {
       cosole.log ('D');
    } else if (score >= 0 && score <= 49) {
      cosole.log ('F');
    } 
}

2. let month = 'april';
    switch (month) {
        case 'september':
        case 'october':
        case 'november':
            console.log ('Autumn');
        case 'december':
        case 'january':
        case 'february':
            console.log ('Winter');
        case 'march':
        case 'april':
        case 'may':
            console.log ('Spring');
        case 'june':
        case 'july':
        case 'august':
            console.log ('Summer');
   }

3. let day = 'saturday'
      switch (day) {
        case 'saturday':
        case 'sunday':
            console.log('(day)is a weekend.`);
        case 'monday':
        case 'tuesday':
        case 'wednesday':
        case 'thursday':
        case 'friday':
           console.log('(day)is a working day.`);
   }
   
Exercise: Level 3:
1. let month = 'may'
   month = month.toLowerCase();
    switch (month) {
        case 'january':
        case 'march':
        case 'may':
        case 'july':
        case 'august':
        case 'october':
        case 'december':
            return 31;
        case 'april':
        case 'june':
        case 'september':
        case 'november':
            return 30;
        case 'February':
            return 28;
    }

3. let month = 'January';
   let year = '2021';
   month = month.toLowerCase();
   if year (year % 4 == 0) {
    switch (month) {
        case 'january':
        case 'march':
        case 'may':
        case 'july':
        case 'august':
        case 'october':
        case 'december':
            return 31;
        case 'april':
        case 'june':
        case 'september':
        case 'november':
            return 30;
        case 'february':
            return 29;
    }
   }elseswitch (month) {
        case 'january':
        case 'march':
        case 'may':
        case 'july':
        case 'august':
        case 'october':
        case 'december':
            return 31;
        case 'april':
        case 'june':
        case 'september':
        case 'november':
            return 30;
        case 'february':
            return 29;
    }

Exercise: Level 2
1. const countries = [
	'USA', 'Canada', 'Germany', 'Australia', 'India'
];

module.exports = countries;

const webTechs = [
    'HTML', 'CSS', 'JavaScript', 'React', 'Node.js'
];

module.exports = webTechs;

const countries = require('./countries');
const webTechs = require('./web_techs');

console.log('Countries:', countries);
console.log('Web Technologies:', webTechs);

2. let text = 'I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.';
let words = text.replace(/[.,\/#!$%\^&\*;:{}=\-_`~()]/g, '').split(' ');
console.log(words);
console.log(words.length);

3. const shoppingCart = ['Milk', 'Coffee', 'Tea', 'Honey'];
if (!shoppingCart.includes('Meat')) {
    shoppingCart.unshift('Meat');
}
if (!shoppingCart.includes('Sugar')) {
    shoppingCart.push('Sugar');
}
const allergicToHoney = true; // Change to false if you are not allergic
if (allergicToHoney) {
    const honeyIndex = shoppingCart.indexOf('Honey');
    if (honeyIndex !== -1) {
        shoppingCart.splice(honeyIndex, 1);
    }
}
const teaIndex = shoppingCart.indexOf('Tea');
if (teaIndex !== -1) {
    shoppingCart[teaIndex] = 'Green Tea';
}

console.log(shoppingCart);

4. const countries = ['USA', 'Canada', 'Germany', 'Australia', 'India'];
if (countries.includes('Ethiopia')) {
    console.log('ETHIOPIA');
} else {
    countries.push('Ethiopia');
    console.log(countries);
}

5. const webTechs = ['HTML', 'CSS', 'JavaScript', 'React', 'Node.js'];
if (webTechs.includes('Sass')) {
    console.log('Sass is a CSS preprocess');
} else {
    webTechs.push('Sass');
    console.log(webTechs);
}

6. const frontEnd = ['HTML', 'CSS', 'JS', 'React', 'Redux'];
const backEnd = ['Node', 'Express', 'MongoDB'];

const fullStack = [...frontEnd, ...backEnd];

console.log(fullStack);

Exercise: Level 3
1. const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24];

ages.sort((a, b) => a - b);

const minAge = ages[0];
const maxAge = ages[ages.length - 1];

let medianAge;
if (ages.length % 2 === 0) {
    medianAge = (ages[Math.floor(ages.length / 2) - 1] + ages[Math.floor(ages.length / 2)]) / 2;
} else {
    medianAge = ages[Math.floor(ages.length / 2)];
}

const sumAges = ages.reduce((acc, age) => acc + age, 0);
const averageAge = sumAges / ages.length;

const rangeAges = maxAge - minAge;

const diffMinAverage = Math.abs(minAge - averageAge);
const diffMaxAverage = Math.abs(maxAge - averageAge);

console.log('Sorted Ages:', ages);
console.log('Min Age:', minAge);
console.log('Max Age:', maxAge);
console.log('Median Age:', medianAge);
console.log('Average Age:', averageAge);
console.log('Range of Ages:', rangeAges);
console.log('Comparison (min - average) vs (max - average):', diffMinAverage, diffMaxAverage);

2. const countries = [
  'Afghanistan', 'Albania', 'Algeria', 'Andorra', 'Angola',
  'Antigua and Barbuda', 'Argentina', 'Armenia', 'Australia', 'Austria',
  'Azerbaijan', 'Bahamas', 'Bahrain', 'Bangladesh', 'Barbados', 'Belarus',
  'Belgium', 'Belize', 'Benin', 'Bhutan', 'Bolivia', 'Bosnia and Herzegovina',
  'Botswana', 'Brazil', 'Brunei', 'Bulgaria', 'Burkina Faso', 'Burundi',
  'Cambodia', 'Cameroon', 'Canada', 'Cape Verde', 'Central African Republic',
  'Chad', 'Chile', 'China', 'Colombi', 'Comoros', 'Congo (Brazzaville)',
  'Congo', 'Costa Rica', "Cote d'Ivoire", 'Croatia', 'Cuba', 'Cyprus',
  'Czech Republic', 'Denmark', 'Djibouti', 'Dominica', 'Dominican Republic',
  'East Timor (Timor Timur)', 'Ecuador', 'Egypt', 'El Salvador',
  'Equatorial Guinea', 'Eritrea', 'Estonia', 'Ethiopia', 'Fiji', 'Finland',
  'France', 'Gabon', 'Gambia, The', 'Georgia', 'Germany', 'Ghana', 'Greece',
  'Grenada', 'Guatemala', 'Guinea', 'Guinea-Bissau', 'Guyana', 'Haiti',
  'Honduras', 'Hungary', 'Iceland', 'India', 'Indonesia', 'Iran', 'Iraq',
  'Ireland', 'Israel', 'Italy', 'Jamaica', 'Japan', 'Jordan', 'Kazakhstan',
  'Kenya', 'Kiribati', 'Korea, North', 'Korea, South', 'Kuwait', 'Kyrgyzstan',
  'Laos', 'Latvia', 'Lebanon', 'Lesotho', 'Liberia', 'Libya', 'Liechtenstein',
  'Lithuania', 'Luxembourg', 'Macedonia', 'Madagascar', 'Malawi', 'Malaysia',
  'Maldives', 'Mali', 'Malta', 'Marshall Islands', 'Mauritania', 'Mauritius',
  'Mexico', 'Micronesia', 'Moldova', 'Monaco', 'Mongolia', 'Morocco',
  'Mozambique', 'Myanmar', 'Namibia', 'Nauru', 'Nepal', 'Netherlands',
  'New Zealand', 'Nicaragua', 'Niger', 'Nigeria', 'Norway', 'Oman', 'Pakistan',
  'Palau', 'Panama', 'Papua New Guinea', 'Paraguay', 'Peru', 'Philippines',
  'Poland', 'Portugal', 'Qatar', 'Romania', 'Russia', 'Rwanda',
  'Saint Kitts and Nevis', 'Saint Lucia', 'Saint Vincent', 'Samoa',
  'San Marino', 'Sao Tome and Principe', 'Saudi Arabia', 'Senegal',
  'Serbia and Montenegro', 'Seychelles', 'Sierra Leone', 'Singapore',
  'Slovakia', 'Slovenia', 'Solomon Islands', 'Somalia', 'South Africa',
  'Spain', 'Sri Lanka', 'Sudan', 'Suriname', 'Swaziland', 'Sweden',
  'Switzerland', 'Syria', 'Taiwan', 'Tajikistan', 'Tanzania', 'Thailand',
  'Togo', 'Tonga', 'Trinidad and Tobago', 'Tunisia', 'Turkey',
  'Turkmenistan', 'Tuvalu', 'Uganda', 'Ukraine', 'United Arab Emirates',
  'United Kingdom', 'United States', 'Uruguay', 'Uzbekistan', 'Vanuatu',
  'Vatican City', 'Venezuela', 'Vietnam', 'Yemen', 'Zambia', 'Zimbabwe'
];

const firstTenCountries = countries.slice(0, 10);

let middleCountries;
if (countries.length % 2 === 0) {
    middleCountries = countries.slice(countries.length / 2 - 1, countries.length / 2 + 1);
} else {
    middleCountries = countries.slice(Math.floor(countries.length / 2), Math.floor(countries.length / 2) + 1);
}

const halfLength = Math.ceil(countries.length / 2);
const firstHalfCountries = countries.slice(0, halfLength);
const secondHalfCountries = countries.slice(halfLength);

console.log('First ten countries:', firstTenCountries);
console.log('Middle country(ies):', middleCountries);
console.log('First half of countries:', firstHalfCountries);
console.log('Second half of countries:', secondHalfCountries);


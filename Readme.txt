1_ fist commit

Tailwind Config Cjs
tailwind.config.cjs are copied from -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/tailwind.config.cjs
The changes contain colours, font and screen resolutions with breakpoints for mobile devices (responsive design)

Index.css
Index.css was also changed with -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/src/index.css 
These changes contain styles to be used with Tailwind

Constants -> index.js -> this will work with ASSETS as images and such and would create CONSTANTS from them, the constants are usefull for users,
they don't need to know how to code, just go there and do some changes.. easy / or add 

Style.js was copied from -> https://github.com/adrianhajdin/project_hoobank/blob/45b4958981ea82423693f6f31524ec8ef08651cb/src/style.js 
This style contain settings fro margins and flexes, layout, this is an important style to understand how aligning and positioning on website works like
collections of class names collected into name strings, so it is easier to use these

Creating components folder, react is all about components

Navbar function: 
${index === navLinks.length -1 ? 'mr-0' : 'mr-10'} - we are setting margin right 10 for each navLink entry, but it is the last entry in the list, then the margin will be 0


/* COPY OF HERO.*/ 


import React from 'react'
import styles from '../style'
import { discount, robot } from '../assets'
import GetStarted from './GetStarted'

const Hero = () => {
  return (
  <section id="home" className={`flex md:flex-row flex-col ${styles.paddingY}`}>
    <div className={`flex-1 ${styles.flexStart} flex-col xl:px-0 sm:px-16 px-6`}>
      <div className='flex flex-row items-center py-[6px] px-4 bg-discount-gradient rounded-[10px] mb-2'>
        <img src={discount} alt="discount" className='w-[32px] h-[32px]'/>
        <p className={`${styles.paragraph} ml-2`}>
          <span className='text-white'>20%</span> Discount for {" "}
          <span className='text-white'>1 Month</span> Account
        </p>
      </div>

      <div className='flex flex-rox justify-between items-center w-full'>
        <h1 className='flex-1 font-poppins font-semibold ss:text-[72px] text-[52px] text-white ss:leading-[100px] leading-[75px]'>
          The Next <br className='sm:block hidden' />{" "}
          <span className='text-gradient'> Generation</span>{" "}
           Payment Method.
        </h1>

        <div className='ss:flex hidden md:mr-4' >
          <GetStarted />
        </div>
      </div>

    </div>
  </section>
  )
}

export default Hero


** EXPORT OF GET STARTED ** - problem on line 74, where MR-2 caused problem with screen width

import styles from '../style'
import { arrowUp } from '../assets'

const GetStarted = () => {
  return (
    <div className={`${styles.flexCenter} w-[140px] h-[140px] rounded-full bg-blue-gradient p-[2px] cursor-pointer`}>
      <div className={`${styles.flexCenter} flex-col bg-primary w-[100%] h-[100%] rounded-full`}>
        <div className={`${styles.flexStart} flex-row`}>
            <p className='font-poppins font-medium text-[18px] leading-[23px] mr-2'>
              <span className='text-gradient'>Get</span>
            </p>
            <img src={arrowUp} alt="arrow up" className='w-[23px] h-[23px] object-contain' />
        </div>

        <p className='font-poppins font-medium text-[18px] leading-[23px]'>
              <span className='text-gradient'>Started</span>
            </p>
      </div>
    </div>
  )
}

export default GetStarted
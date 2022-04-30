# Command C Command V

I partially copied some code from youtube that 
auto-swipes on tinder. Here are the details:

    bot = TinderBot()

    bot.driver.get('https://tinder.com')

    lg_btn = bot.driver.find_element_by_xpath('//*[@id="content"]/div/div[1]/div/main/div[1]/div/div/div/div/header/div/div[2]/div[2]/button/span')
    lg_btn.click()

    fb_btn = bot.driver.find_element_by_xpath('//*[@id="modal-manager"]/div/div/div[1]/div/div[3]/span/div[2]/button')

    fb_btn.click()

    base_window = bot.driver.window_handles[0]

    bot.driver.switch_to_window(bot.driver.window_handles[1])

    email_in = bot.driver.find_element_by_xpath('//*[@id="email"]')

    email_in.send_keys('nate18974@gmail.com')

    pw_in = bot.driver.find_element_by_xpath('//*[@id="pass"]')

    pw_in.send_keys('Natester1')

    login_btn = bot.driver.find_element_by_xpath('//*[@id="u_0_0"]')

    login_btn.click()

    continue_btn = bot.driver.find_element_by_xpath('//*[@id="u_0_4"]/div[2]/div[2]/div[1]/button')

    continue_btn.click()




    like_btn = bot.driver.find_element_by_xpath('//*[@id="t-1890905246"]/div/div[1]/div/div/main/div/div[1]/div/div[2]/div[4]/button')

      while True:
        sleep(0.5)
        try:
          like_btn.click()
        except Exception:
          try:
            popup_btn = bot.driver.find_element_by_xpath('//*[@id="modal-manager"]/div/div/button[2]')
            popup_btn.click()

          except Exception:
            close_mch = bot.driver.find_element_by_xpath('')
            close_mch.click()


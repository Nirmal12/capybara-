
click_link('Login')
sleep 5
facebook_window = window_opened_by do
	click_button('LOGIN WITH FACEBOOK')
end
sleep 3
within_window facebook_window do
  find('#email').set('xxxxx@yahoo.com')
  find('#pass').set('xxxx')
  click_button 'Log In'
end
sleep 10
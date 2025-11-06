# Coolbet Chile - Test Scenarios Document

**Platform:** https://www.coolbetchile.com/
**Document Version:** 2.1
**Date:** November 6, 2025
**Last Updated:** November 6, 2025 - Updated with actual registration form fields
**Test Type:** Functional Testing - Success Scenarios

---

## Important Testing Guidelines

### 📸 Screenshot Requirements
**CRITICAL: Take screenshots at EVERY step of the testing process**

- Capture screenshots for each action performed
- Include screenshots of all confirmation messages
- Document all error messages (if any occur)
- Screenshot all email confirmations received
- Capture final results and account status changes
- Save screenshots with clear naming: `TC-[TestID]-Step-[Number]-[Description].png`
- Example: `TC-REG-001-Step-05-Registration-Success.png`

### General Notes
- Test data values are not specified - use realistic Chilean data
- KYC verification may be required at different stages - complete when prompted
- All amounts should be in Chilean Pesos (CLP)
- Test on the actual platform, not a demo/sandbox environment
- Record any deviations or unexpected behavior

---

## 1. REGISTRATION TEST SCENARIO

### TC-REG-001: New User Registration

**Objective:** Successfully register a new user account on Coolbet Chile

**Preconditions:**
- Valid email address (not previously registered)
- Must be 18+ years old
- Valid Chilean RUT (Chilean national identification number)
- Valid Chilean mobile phone number (for SMS verification)
- Valid Chilean address (street, city, zip code)
- Have ready: First name, Father's last name, Mother's last name (or single family name)
- Decide on a username/alias (minimum 6 characters)

**Test Steps:**

**STEP 1: Initial Registration Form**

1. Navigate to https://www.coolbetchile.com/
   - **📸 Screenshot:** Homepage

2. Locate and click the Registration button or scroll to the registration form
   - Form may be directly visible on homepage
   - Or look for "Registrarse", "Registro", "Crear Cuenta" button
   - **📸 Screenshot:** Registration form location

3. Fill in the Email / Password section:
   - **Email:** Enter a valid email address (not previously registered)
   - **Password:** Create a password (note: password requirements may apply)
   - **📸 Screenshot:** Email and password entered

4. Fill in the Mobile phone section:
   - **Country Code:** Should be pre-selected as +56 (Chile)
   - **Mobile number:** Enter valid Chilean mobile phone number
   - Note the message: "Please use a valid mobile phone number. It will be used to send you a verification SMS"
   - **📸 Screenshot:** Mobile phone number entered

5. Verify Country and Currency settings:
   - **Country:** Chile (with flag icon) should be selected
   - **Currency:** CLP (Chilean Peso) should be selected
   - **📸 Screenshot:** Country and currency settings

6. Accept all required checkboxes (all are mandatory):
   - ☑ "I confirm that I am at least 18 years old and that I am playing on my own behalf"
   - ☑ "I agree to the Terms, and have read the Privacy Policy, including the Cookie Policy"
   - ☑ "I consent to my data being shared with advertisers and social media platforms for targeted advertising"
   - **📸 Screenshot:** All three checkboxes checked

7. Review the gambling warning message:
   - "Attention! Gambling can be addictive! Play responsibly!"
   - **📸 Screenshot:** Complete form ready for submission

8. Click the green "REGISTER" button
   - **📸 Screenshot:** After clicking Register

**STEP 2: Contact Information Form (USER INFO → CONTACT INFO)**

9. You should now see a progress bar with three steps:
   - USER INFO (completed - green checkmark)
   - CONTACT INFO (current - active)
   - SMS VERIFICATION (pending)
   - **📸 Screenshot:** Progress indicator showing CONTACT INFO step

10. Fill in Personal Name information:
    - **First name:** Enter your first name
    - **Father's last name:** Enter your father's last name (apellido paterno)
    - **Mother's last name:** Enter your mother's last name (apellido materno)
    - **Toggle option:** "I only have one family name" - use if applicable (leave OFF for standard two last names)
    - **📸 Screenshot:** Name fields completed

11. Select Gender:
    - Choose either MALE or FEMALE radio button
    - **📸 Screenshot:** Gender selected

12. Enter RUT code:
    - **RUT code:** Enter your Chilean national identification number (RUT)
    - Format: XXXXXXXX-X
    - **📸 Screenshot:** RUT entered

13. Enter Date of Birth:
    - **Birth year:** Select from dropdown
    - **Month:** Select from dropdown
    - **Day:** Select from dropdown
    - Ensure you are 18+ years old
    - **📸 Screenshot:** Date of birth selected

14. Enter Address information:
    - **Address Line 1:** Street name and house number
    - **Address Line 2 (optional):** Apartment, suite or space number (if applicable)
    - **Zip Code:** Enter postal code
    - **City:** Enter city name
    - **📸 Screenshot:** Address fields completed

15. Enter Alias:
    - **Alias:** Create a username/alias (minimum 6 characters)
    - **📸 Screenshot:** Alias entered

16. Choose bonus offers preference:
    - Question: "Do you want to receive bonus offers, free spins and promotion?"
    - Select either YES or NO
    - **📸 Screenshot:** Bonus preference selected

17. Review all information in the Contact Info form:
    - **📸 Screenshot:** Complete Contact Info form ready for submission

18. Click the green "CREATE ACCOUNT" button
    - **📸 Screenshot:** After clicking Create Account

**STEP 3: SMS Verification**

19. You should proceed to SMS VERIFICATION step:
    - Progress bar should show: USER INFO ✓ → CONTACT INFO ✓ → SMS VERIFICATION (active)
    - **📸 Screenshot:** SMS verification screen

20. Check your mobile phone for verification SMS:
    - **📸 Screenshot:** SMS received on phone (if possible)

21. Enter the SMS verification code:
    - Enter the code from the SMS
    - **📸 Screenshot:** Verification code entered

22. Confirm the SMS verification:
    - Click Submit/Verify button
    - **📸 Screenshot:** Verification confirmation

**STEP 4: Confirm Registration Complete**

23. Check for email confirmation:
    - Check your email inbox for welcome/confirmation email
    - **📸 Screenshot:** Confirmation email received

24. Verify registration is complete:
    - You should be logged in or prompted to login
    - Account dashboard should be accessible
    - **📸 Screenshot:** Account dashboard or confirmation of successful registration

25. Verify account status:
    - Check that you can see your account balance
    - Verify your username/alias is displayed
    - **📸 Screenshot:** Full account view showing successful registration

**Expected Results:**

**Step 1 - Initial Form:**
- ✅ Registration form loads correctly with all fields visible
- ✅ Email, password, and mobile phone fields accept input
- ✅ Country is pre-selected as Chile with +56 code
- ✅ Currency is set to CLP
- ✅ All three checkboxes are mandatory and functional
- ✅ Social login options visible (Facebook, Google, Apple)
- ✅ "DEPOSIT & PLAY" quick signup option available at top
- ✅ Register button is clickable when form is complete

**Step 2 - Contact Info Form:**
- ✅ Progress bar displays correctly (USER INFO → CONTACT INFO → SMS VERIFICATION)
- ✅ All name fields (First name, Father's last name, Mother's last name) accept input
- ✅ "I only have one family name" toggle works if needed
- ✅ Gender selection (Male/Female) works properly
- ✅ RUT code field accepts Chilean RUT format
- ✅ Date of birth dropdowns function correctly (Birth year, Month, Day)
- ✅ Address fields accept input (Address Line 1, Line 2, Zip Code, City)
- ✅ Alias field enforces minimum 6 characters
- ✅ Bonus offers question (YES/NO) is selectable
- ✅ "CREATE ACCOUNT" button is clickable when form is complete

**Step 3 - SMS Verification:**
- ✅ SMS verification code is sent to mobile phone
- ✅ SMS arrives within reasonable time (1-2 minutes)
- ✅ Verification code entry field is displayed
- ✅ Code is accepted and verified successfully
- ✅ Progress advances to completion

**Step 4 - Registration Complete:**
- ✅ Confirmation message displayed
- ✅ Welcome/confirmation email received
- ✅ User account is created and active
- ✅ User is logged in automatically or can login
- ✅ Account dashboard accessible
- ✅ Username/alias displayed correctly
- ✅ Account balance visible (should be 0 CLP initially)

**Post-Test:**
- **Record:** Email used for registration
- **Record:** Mobile phone number used
- **Record:** Username/Alias created
- **Record:** RUT number used
- **Record:** Any account number or user ID assigned
- **Record:** Registration method used (standard form or social login if tested)

---

### TC-REG-002: Alternative Registration Methods (Optional Testing)

**Objective:** Test alternative registration methods available on Coolbet Chile

**Alternative Methods Available:**

**A) DEPOSIT & PLAY (Trustly Quick Signup)**
- Green button at top of registration form: "DEPOSIT & PLAY"
- Text: "SIGN UP QUICKLY THROUGH TRUSTLY BY CLICKING DEPOSIT & PLAY"
- This method allows instant signup through Trustly payment service
- Registration and deposit happen in one step
- **Test if time permits:** Click this button and follow Trustly flow

**B) Social Login Options**
Three social login methods are available at bottom of form:
1. **FACEBOOK** - Login/Register via Facebook account
2. **GOOGLE** - Login/Register via Google account
3. **APPLE** - Login/Register via Apple ID

**Testing Social Login (if desired):**
1. Select one of the social login options
2. Authorize Coolbet Chile to access your social account
3. Complete any additional required information
4. Verify account is created and functional
5. **📸 Screenshot:** Each step of social login process

**Note:** These alternative methods are optional tests. The standard registration form (TC-REG-001) is the primary test case.

---

## 2. LOGIN TEST SCENARIO

### TC-LOG-001: User Login

**Objective:** Successfully login to an existing Coolbet Chile account

**Preconditions:** 
- User account must already be registered
- Email must be verified (if verification was required)
- You have correct login credentials

**Test Steps:**

1. Navigate to https://www.coolbetchile.com/
   - **📸 Screenshot:** Homepage

2. Locate and click the Login button (may be labeled "Iniciar Sesión", "Login", "Ingresar", or similar)
   - **📸 Screenshot:** Login button location

3. Enter your registered email address in the email/username field
   - **📸 Screenshot:** Email entered

4. Enter your password in the password field
   - Note: Password should be masked (dots or asterisks)
   - **📸 Screenshot:** Password field filled (masked)

5. (Optional) If there is a "Remember Me" checkbox, you may check it for testing purposes
   - **📸 Screenshot:** Remember Me option (if available)

6. Click the Login/Sign In button
   - **📸 Screenshot:** Login button clicked

7. Wait for login process to complete
   - **📸 Screenshot:** Successful login - account dashboard/homepage

8. Verify you are logged in:
   - Check for your username/account name displayed
   - Verify account menu is accessible
   - Confirm account balance is visible
   - **📸 Screenshot:** Full logged-in dashboard view

**Expected Results:**
- ✅ Login form accepts credentials
- ✅ Login successful
- ✅ User redirected to account area
- ✅ Username/account info displayed
- ✅ Account balance visible
- ✅ All account features accessible

**Post-Test:**
- **Record:** Current account balance
- **Record:** Account status (any notifications or pending actions)

---

## 3. KYC VERIFICATION (OPTIONAL - COMPLETE WHEN REQUIRED)

### TC-KYC-001: KYC Document Verification

**Objective:** Complete KYC (Know Your Customer) verification when required

**IMPORTANT NOTES:**
- KYC may be required at different stages:
  - After registration
  - Before first deposit
  - Before withdrawal
  - After reaching certain betting limits
- Complete this test scenario whenever the platform prompts for KYC
- If KYC is not immediately required, skip this section and return to it when prompted

**Preconditions:** 
- User is logged in
- Platform is requesting KYC verification
- You have required documents ready (valid and current)

**Required Documents (Typical):**
- Chilean National ID (Cédula de Identidad) - Front side
- Chilean National ID (Cédula de Identidad) - Back side  
- Proof of Address (utility bill or bank statement less than 3 months old)
- Selfie with ID (may be required)

**Test Steps:**

1. When prompted for KYC verification, locate the verification section
   - This may appear as a popup, banner, or in account settings
   - May be labeled "Verificar Cuenta", "Verificación", "KYC", or similar
   - **📸 Screenshot:** KYC prompt/notification

2. Click to start the verification process
   - **📸 Screenshot:** KYC upload page

3. Review the document requirements listed
   - **📸 Screenshot:** Document requirements shown

4. Upload Front side of Chilean ID:
   - Click the upload button/area for front ID
   - Select your ID front image file (ensure it is clear, not blurry)
   - File formats typically accepted: JPG, PNG, PDF
   - File size should be under 5MB
   - **📸 Screenshot:** Front ID uploaded successfully

5. Upload Back side of Chilean ID:
   - Click the upload button/area for back ID
   - Select your ID back image file
   - **📸 Screenshot:** Back ID uploaded successfully

6. Upload Proof of Address document:
   - Click the upload button/area for address proof
   - Select your document (utility bill, bank statement, etc.)
   - Ensure document clearly shows: your name, address, and recent date
   - **📸 Screenshot:** Address proof uploaded successfully

7. Upload Selfie with ID (if required):
   - If requested, take or upload a selfie holding your ID
   - Ensure both your face and ID are clearly visible
   - **📸 Screenshot:** Selfie uploaded successfully

8. Review all uploaded documents:
   - Check that all required documents are uploaded
   - Verify thumbnails/previews are visible
   - **📸 Screenshot:** All documents uploaded - ready to submit

9. Click Submit/Send for Verification button
   - **📸 Screenshot:** Submission confirmation message

10. Note the verification status:
    - Status should change to "Under Review" or "Pending"
    - **📸 Screenshot:** KYC status after submission

11. Check email for confirmation:
    - You should receive an email confirming documents received
    - **📸 Screenshot:** Email confirmation

12. Wait for review to complete (typically 24-48 hours):
    - Check back periodically or wait for email notification
    - **📸 Screenshot:** Approval email when received

13. Verify KYC approval in account:
    - Login to account
    - Check verification status - should show "Verified" or similar
    - Look for verification badge/checkmark
    - **📸 Screenshot:** Account showing verified status

**Expected Results:**
- ✅ All documents upload successfully
- ✅ Accepted file formats work correctly
- ✅ Submission confirmed
- ✅ Confirmation email received
- ✅ Status changes to "Under Review"
- ✅ Within 24-48 hours: KYC approved
- ✅ Approval email received
- ✅ Account status shows "Verified"
- ✅ Full platform functionality unlocked
- ✅ Can now proceed with deposits and withdrawals

**Post-Test:**
- **Record:** Verification status
- **Record:** Time taken for approval
- **Record:** Any new limits or features unlocked

**If KYC is Rejected:**
- **📸 Screenshot:** Rejection notification
- **Record:** Rejection reason provided
- Re-upload corrected documents as needed
- Document the re-submission process

---

## 4. DEPOSIT TEST SCENARIO

### TC-DEP-001: Minimum Deposit

**Objective:** Successfully deposit the minimum allowed amount to the account

**Preconditions:** 
- User is logged in
- KYC verification completed (if required for deposits)
- Valid payment method available

**Test Steps:**

1. From your account dashboard, locate and click the Deposit button/link
   - May be labeled "Depositar", "Deposit", "Recargar", or similar
   - **📸 Screenshot:** Deposit button location

2. Review available deposit methods:
   - Credit/Debit Card
   - Bank Transfer
   - Digital Wallets (Mercado Pago, MACH, etc.)
   - Other local payment methods
   - **📸 Screenshot:** All available deposit methods

3. Select your preferred deposit method:
   - Click on the payment method you will use
   - **📸 Screenshot:** Selected payment method

4. Review the minimum and maximum deposit limits displayed:
   - Note the minimum amount allowed
   - **📸 Screenshot:** Deposit limits shown

5. Enter the MINIMUM deposit amount:
   - Enter the exact minimum amount allowed (e.g., if minimum is 5,000 CLP, enter 5,000)
   - **📸 Screenshot:** Minimum amount entered

6. Review any fees or charges (if applicable):
   - Check if processing fees are shown
   - **📸 Screenshot:** Fee breakdown (if any)

7. Enter payment details as required:
   - For cards: card number, expiry, CVV, cardholder name
   - For bank transfer: follow instructions provided
   - For digital wallets: you may be redirected to wallet app/website
   - **📸 Screenshot:** Payment details entry screen (mask sensitive information)

8. Review the transaction summary before confirming:
   - Deposit amount
   - Payment method
   - Total to be charged
   - **📸 Screenshot:** Transaction summary

9. Click Confirm/Process Payment button:
   - **📸 Screenshot:** Confirmation button

10. Complete any additional verification:
    - 3D Secure authentication (for cards) - enter OTP if prompted
    - Wallet authentication - authorize in app
    - **📸 Screenshot:** Additional authentication step (if applicable)

11. Wait for transaction processing:
    - Processing indicator should appear
    - **📸 Screenshot:** Processing screen

12. Verify deposit confirmation:
    - Success message should appear
    - Transaction ID or reference number provided
    - **📸 Screenshot:** Deposit success confirmation

13. Check account balance update:
    - Balance should increase by deposit amount
    - **📸 Screenshot:** Updated account balance

14. Verify transaction in history:
    - Go to transaction history/account statement
    - Locate the deposit transaction
    - Verify: date, time, amount, method, status (completed)
    - **📸 Screenshot:** Deposit in transaction history

15. Check email confirmation:
    - Email should be sent confirming the deposit
    - **📸 Screenshot:** Deposit confirmation email

**Expected Results:**
- ✅ Deposit page loads correctly
- ✅ All payment methods displayed
- ✅ Minimum/maximum limits clearly shown
- ✅ Minimum amount accepted
- ✅ Payment processed successfully
- ✅ Transaction confirmed with reference number
- ✅ Funds credited to account immediately (or within stated timeframe)
- ✅ Account balance updated correctly
- ✅ Transaction appears in history
- ✅ Confirmation email received

**Post-Test:**
- **Record:** Deposit amount
- **Record:** Payment method used
- **Record:** Transaction ID/Reference number
- **Record:** New account balance
- **Record:** Any processing fees charged
- **Record:** Time taken for funds to appear

---

## 5. PLACE A BET - CASINO/SLOT TEST SCENARIO

### TC-BET-001: Place Bet on Slot Machine

**Objective:** Successfully place bets on a casino slot machine game

**Preconditions:** 
- User is logged in
- Account has sufficient balance (from deposit)
- Account is verified (if required for casino access)

**Test Steps:**

1. From your account dashboard, locate and click on the Casino section:
   - May be labeled "Casino", "Slots", "Juegos", or similar
   - **📸 Screenshot:** Casino section button/link

2. Browse the casino lobby:
   - Review available slot machines/games
   - **📸 Screenshot:** Casino game lobby

3. Choose any slot machine game:
   - Select a game that interests you
   - Popular providers: Pragmatic Play, NetEnt, Evolution, etc.
   - **📸 Screenshot:** Selected slot game

4. Click to open/launch the slot game:
   - Game may open in same window or new window
   - Wait for game to load completely
   - **📸 Screenshot:** Game loading screen

5. Review the game interface when loaded:
   - Game screen
   - Spin button
   - Bet amount selector
   - Balance display
   - Game information/paytable (if visible)
   - **📸 Screenshot:** Fully loaded slot game interface

6. Check your current balance in the game:
   - Balance should match your account balance
   - **📸 Screenshot:** Balance displayed in game

7. Set your bet amount:
   - Locate bet amount controls (usually +/- buttons or bet selector)
   - You can start with minimum bet or adjust as preferred
   - **📸 Screenshot:** Bet amount selected

8. Review game bet settings:
   - Bet per line (if applicable)
   - Number of lines (if applicable)
   - Total bet amount
   - **📸 Screenshot:** Bet configuration

9. Place your first bet by clicking the Spin button:
   - **📸 Screenshot:** Spin button clicked / Game in action

10. Wait for spin to complete:
    - Watch the reels spin and stop
    - **📸 Screenshot:** Spin result (win or lose)

11. Check result of first spin:
    - Note if you won or lost
    - Check balance update
    - **📸 Screenshot:** Balance after first spin

12. Place additional bets (minimum 5 total spins):
    - Spin 2: **📸 Screenshot:** Result
    - Spin 3: **📸 Screenshot:** Result  
    - Spin 4: **📸 Screenshot:** Result
    - Spin 5: **📸 Screenshot:** Result

13. Review game history (if available in game):
    - Some slots show recent spins history
    - **📸 Screenshot:** Game history (if available)

14. Note your final balance after all spins:
    - **📸 Screenshot:** Final balance in game

15. Exit the game:
    - Click back/exit button
    - Return to casino lobby or main account area
    - **📸 Screenshot:** Returning to main platform

16. Verify account balance on main platform:
    - Balance should reflect all bets placed
    - **📸 Screenshot:** Account balance after casino gaming

17. Check betting history/transaction history:
    - Navigate to account history
    - Locate casino game transactions
    - Verify all bets are recorded
    - **📸 Screenshot:** Casino bets in transaction history

**Expected Results:**
- ✅ Casino section accessible
- ✅ Slot games load properly
- ✅ Game interface displays correctly
- ✅ Balance syncs with account
- ✅ Bet controls work properly
- ✅ Spin button responsive
- ✅ Game plays smoothly without errors
- ✅ Results display clearly
- ✅ Balance updates in real-time after each spin
- ✅ Win amounts credited correctly (if any wins)
- ✅ All bets recorded in transaction history
- ✅ Can exit game and return to platform
- ✅ Final balance accurate

**Post-Test:**
- **Record:** Slot game name
- **Record:** Starting balance
- **Record:** Bet amount per spin
- **Record:** Number of spins played
- **Record:** Total amount wagered
- **Record:** Any wins received
- **Record:** Final balance
- **Record:** Net profit/loss

**Additional Testing (Optional):**
- Try different slot games
- Test different bet amounts
- Test autoplay feature (if available)
- Test game features (free spins, bonus rounds, etc.)

---

## 6. WITHDRAWAL TEST SCENARIO

### TC-WDR-001: Withdraw Funds to Bank Account

**Objective:** Successfully withdraw funds from account to bank account

**Preconditions:** 
- User is logged in
- KYC verification MUST be completed and approved
- Account has sufficient withdrawable balance
- No active wagering requirements or bonus locks
- Bank account details available

**IMPORTANT:** If KYC is not yet completed, you must complete TC-KYC-001 before proceeding with withdrawal.

**Test Steps:**

1. From your account dashboard, locate and click the Withdrawal button/link:
   - May be labeled "Retirar", "Withdrawal", "Retiro", or similar
   - **📸 Screenshot:** Withdrawal button location

2. Review withdrawal requirements or restrictions (if any displayed):
   - KYC status
   - Minimum withdrawal amount
   - Any pending wagering requirements
   - **📸 Screenshot:** Withdrawal page requirements

3. Review available withdrawal methods:
   - Bank Transfer
   - Digital Wallets
   - Other available methods
   - **📸 Screenshot:** Available withdrawal methods

4. Select your preferred withdrawal method:
   - Most common: Bank Transfer
   - Click on your chosen method
   - **📸 Screenshot:** Selected withdrawal method

5. Enter or verify bank account details:
   - If first-time withdrawal: enter bank account information
   - Bank name
   - Account type (Checking/Savings - Cuenta Corriente/Cuenta Vista)
   - Account number
   - Account holder name (must match your registered name)
   - Your RUT
   - If previously saved: verify details are correct
   - **📸 Screenshot:** Bank account details (mask account number for security)

6. Review minimum and maximum withdrawal limits:
   - Note the minimum withdrawal amount
   - **📸 Screenshot:** Withdrawal limits displayed

7. Enter withdrawal amount:
   - Enter the amount you wish to withdraw
   - Amount must be within limits and not exceed your withdrawable balance
   - **📸 Screenshot:** Withdrawal amount entered

8. Review any fees or processing information:
   - Check for withdrawal fees (if any)
   - Review processing time estimate
   - **📸 Screenshot:** Fee and processing time info

9. Review withdrawal summary:
   - Amount to withdraw
   - Destination (bank account)
   - Any fees
   - Net amount you will receive
   - Estimated processing time
   - **📸 Screenshot:** Withdrawal summary

10. Complete any additional verification:
    - 2FA code (SMS/Email) if prompted
    - Security questions if prompted
    - **📸 Screenshot:** 2FA or security verification (if required)

11. Click Confirm/Submit Withdrawal button:
    - **📸 Screenshot:** Confirmation button

12. Wait for withdrawal processing:
    - **📸 Screenshot:** Processing screen

13. Verify withdrawal submission confirmation:
    - Success message should appear
    - Transaction ID or reference number provided
    - Status should show "Pending" or "Processing"
    - **📸 Screenshot:** Withdrawal request confirmation

14. Check account balance:
    - Withdrawal amount should be deducted or marked as "pending"
    - **📸 Screenshot:** Updated account balance

15. Verify transaction in history:
    - Go to transaction history
    - Locate the withdrawal transaction
    - Verify: date, time, amount, method, status
    - **📸 Screenshot:** Withdrawal in transaction history

16. Check email confirmation:
    - Email should be sent confirming withdrawal request
    - **📸 Screenshot:** Withdrawal confirmation email

17. Wait for withdrawal to complete (1-5 business days typically):
    - Monitor withdrawal status in platform
    - **📸 Screenshot:** Updated status if it changes (e.g., from Pending to Processing to Completed)

18. Verify funds received in bank account:
    - Check your bank account after the processing period
    - Confirm funds arrived
    - **📸 Screenshot:** Bank statement showing credit (mask sensitive details)

19. Verify final status in platform:
    - Login to Coolbet
    - Check transaction history
    - Status should be "Completed"
    - **📸 Screenshot:** Final completed status

**Expected Results:**
- ✅ Withdrawal page accessible
- ✅ KYC verification confirmed as completed
- ✅ Withdrawal methods displayed
- ✅ Bank account details can be entered/saved
- ✅ Withdrawal limits clearly shown
- ✅ Amount validation works correctly
- ✅ Withdrawal submitted successfully
- ✅ Confirmation message and transaction ID provided
- ✅ Account balance updated immediately (amount reserved/deducted)
- ✅ Transaction appears in history with "Pending" status
- ✅ Confirmation email received
- ✅ Within stated timeframe (1-5 business days): funds arrive in bank
- ✅ Transaction status updated to "Completed"
- ✅ Amount received matches withdrawal (minus any fees)

**Post-Test:**
- **Record:** Withdrawal amount requested
- **Record:** Withdrawal method used
- **Record:** Transaction ID/Reference number
- **Record:** Bank account used (last 4 digits only)
- **Record:** Stated processing time
- **Record:** Actual processing time (when funds arrived)
- **Record:** Any fees charged
- **Record:** Final amount received in bank
- **Record:** Any issues or delays encountered

---

## 7. END-TO-END TEST SCENARIO

### TC-E2E-001: Complete User Journey

**Objective:** Execute complete user journey from registration through withdrawal

**This is a comprehensive test that combines all previous test cases in sequence.**

**Test Flow:**

1. ✅ **REGISTRATION** (TC-REG-001)
   - Register new user account
   - Verify email if required
   - **📸 Screenshots:** As per TC-REG-001

2. ✅ **LOGIN** (TC-LOG-001)
   - Login with newly created account
   - **📸 Screenshots:** As per TC-LOG-001

3. ⚠️ **KYC VERIFICATION** (TC-KYC-001 - If Required)
   - Complete KYC if prompted at this stage
   - If not required yet, proceed to next step
   - Return to KYC when prompted later
   - **📸 Screenshots:** As per TC-KYC-001 (when completed)

4. ✅ **DEPOSIT** (TC-DEP-001)
   - Make minimum deposit
   - Verify funds credited
   - **📸 Screenshots:** As per TC-DEP-001

5. ⚠️ **KYC VERIFICATION** (TC-KYC-001 - If Required)
   - If KYC not completed earlier and now required, complete it
   - **📸 Screenshots:** As per TC-KYC-001 (when completed)

6. ✅ **PLACE BETS** (TC-BET-001)
   - Play casino slot games
   - Place multiple bets
   - **📸 Screenshots:** As per TC-BET-001

7. ⚠️ **KYC VERIFICATION** (TC-KYC-001 - If Required)
   - If KYC still not done and required before withdrawal, complete it now
   - **📸 Screenshots:** As per TC-KYC-001 (when completed)

8. ✅ **WITHDRAWAL** (TC-WDR-001)
   - Withdraw remaining funds
   - Verify withdrawal processed
   - **📸 Screenshots:** As per TC-WDR-001

**Expected Results:**
- ✅ All steps complete successfully in sequence
- ✅ Smooth transitions between functions
- ✅ KYC completed at whatever stage required
- ✅ All notifications received
- ✅ All transactions recorded accurately
- ✅ Balances remain accurate throughout
- ✅ Complete user lifecycle verified

**Post-Test Documentation:**
- **Summary Report:** Create a summary of the complete journey
- **Screenshots:** Organize all screenshots in chronological order
- **Issues:** Document any issues encountered at any stage
- **Timing:** Record total time for complete journey
- **Notes:** Any observations or recommendations

---

## Test Execution Checklist

Before starting tests:
- [ ] Clear browser cache and cookies
- [ ] Prepare valid Chilean personal data (RUT, phone, address)
- [ ] Have valid ID documents ready (for KYC)
- [ ] Have payment method ready (for deposit)
- [ ] Have bank account details ready (for withdrawal)
- [ ] Create folder structure for organizing screenshots
- [ ] Ensure stable internet connection

During testing:
- [ ] Take screenshot at EVERY step
- [ ] Name screenshots clearly
- [ ] Record all transaction IDs/reference numbers
- [ ] Note exact times for all actions
- [ ] Document any error messages
- [ ] Save all email confirmations

After testing:
- [ ] Organize all screenshots by test case
- [ ] Complete test results documentation
- [ ] Calculate total time for each test
- [ ] Document any deviations from expected results
- [ ] Prepare summary report

---

## Test Results Template

For each test case, document:

**Test Case ID:** [TC-XXX-001]  
**Date Executed:** [Date]  
**Tester Name:** [Name]  
**Browser/Device:** [Chrome/Firefox/Mobile]  
**Test Result:** [PASS / FAIL / BLOCKED]

**Execution Details:**
- Start Time: [Time]
- End Time: [Time]  
- Duration: [Minutes]

**Test Data Used:**
- [Relevant data: amounts, IDs, etc.]

**Screenshots Captured:** [Number of screenshots]  
**Screenshots Location:** [Folder path]

**Actual Results:**
- [Describe what actually happened]

**Deviations from Expected Results:**
- [None / List any differences]

**Issues Encountered:**
- [None / List any problems]

**Additional Notes:**
- [Any observations or comments]

---

## Screenshot Organization

Suggested folder structure:
```
Coolbet_Testing_[Date]/
├── TC-REG-001_Registration/
│   ├── Step-01-Homepage.png
│   ├── Step-02-Register-Button.png
│   └── ...
├── TC-LOG-001_Login/
│   ├── Step-01-Homepage.png
│   └── ...
├── TC-KYC-001_Verification/
│   └── ...
├── TC-DEP-001_Deposit/
│   └── ...
├── TC-BET-001_Casino_Betting/
│   └── ...
├── TC-WDR-001_Withdrawal/
│   └── ...
└── Test_Summary_Report.pdf
```

---

## Final Deliverables

After completing all tests, provide:

1. **Screenshot Package:** All screenshots organized by test case
2. **Test Results Summary:** Document with results for each test case
3. **Transaction Log:** List of all transactions with IDs and amounts
4. **Issues Log:** Any problems encountered during testing
5. **Timing Report:** Duration for each test case
6. **Recommendations:** Suggestions for improvements (if any)

---

**Document Control:**
Version: 2.1 - Updated with Actual Registration Form Fields
Previous Version: 2.0 - Practical Testing Version
Date: November 6, 2025
Status: Ready for Execution

**Version 2.1 Updates:**
- Updated TC-REG-001 with actual multi-step registration process
- Added detailed field descriptions from real registration forms
- Documented 3-step process: Initial Form → Contact Info → SMS Verification
- Added Chilean-specific fields: Father's/Mother's last names, RUT format, Chilean address
- Added TC-REG-002 for alternative registration methods (Trustly, Social Login)
- Enhanced preconditions with complete requirements list
- Added step-by-step screenshots requirements for each registration stage

**Important Reminders:**
- 📸 Screenshot EVERYTHING
- Complete KYC whenever required
- Use minimum deposit amount
- Test casino slots (easier than sports betting)
- Document all transaction IDs
- Keep all email confirmations
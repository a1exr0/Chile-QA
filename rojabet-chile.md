# Rojabet Chile - Test Scenarios Document

**Platform:** https://rojabet.com/
**Document Version:** 1.0
**Date:** November 6, 2025
**Test Type:** Functional Testing - Success Scenarios Only

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
- Focus on SUCCESS scenarios only (positive testing)

---

## 1. REGISTRATION TEST SCENARIO

### TC-REG-001: New User Registration

**Objective:** Successfully register a new user account on Rojabet Chile

**Preconditions:**
- Valid email address (not previously registered)
- Must be 18+ years old
- Valid Chilean RUT (Chilean national identification number)
- Valid Chilean mobile phone number
- Valid Chilean address
- Have personal information ready (name, date of birth, etc.)

**Test Steps:**

1. Navigate to https://rojabet.com/
   - **📸 Screenshot:** Homepage

2. Locate and click the Registration button
   - Look for "Registrarse", "Registro", "Crear Cuenta", or similar
   - May be in top right corner or prominent on homepage
   - **📸 Screenshot:** Registration button location

3. Registration form should appear
   - **📸 Screenshot:** Registration form displayed

4. Fill in all required personal information fields:
   - **Email address:** Enter valid email (not previously used)
   - **Password:** Create strong password (note any requirements shown)
   - **Confirm Password:** Re-enter password
   - **First Name (Nombre):** Enter your first name
   - **Last Name (Apellido):** Enter your last name(s)
   - **RUT:** Enter Chilean national identification number
   - **Date of Birth:** Enter DOB (ensure you are 18+)
   - **Gender:** Select gender if required
   - **Mobile Phone:** Enter Chilean phone number
   - **Address:** Enter street address
   - **City:** Enter city
   - **Postal Code:** Enter zip/postal code
   - **Any other mandatory fields marked with asterisk (*)**
   - **📸 Screenshot:** Completed registration form (before submission)

5. Review and accept required checkboxes:
   - ☑ Terms and Conditions agreement
   - ☑ Privacy Policy agreement
   - ☑ Age confirmation (18+ years old)
   - ☑ Responsible gaming acknowledgment
   - ☑ Any other mandatory agreements
   - **📸 Screenshot:** All required checkboxes checked

6. Review promotional/marketing preferences (if applicable):
   - Choose whether to receive promotional emails/SMS
   - **📸 Screenshot:** Marketing preferences selected

7. Click the Submit/Register button
   - Button may say "Registrarse", "Crear Cuenta", "Register", or similar
   - **📸 Screenshot:** After clicking Submit

8. Wait for registration processing
   - **📸 Screenshot:** Processing indicator (if visible)

9. Check for email verification requirement:
   - Check your email inbox for verification email
   - **📸 Screenshot:** Verification email received
   - Click the verification link in the email
   - **📸 Screenshot:** Email verification success page

10. Check for phone/SMS verification requirement:
    - If SMS verification is required, check your phone
    - **📸 Screenshot:** SMS received (if possible)
    - Enter verification code if prompted
    - **📸 Screenshot:** SMS verification screen

11. Verify registration success:
    - Success message should be displayed
    - You may be automatically logged in
    - Or you may be prompted to login
    - **📸 Screenshot:** Registration success confirmation

12. Access your account:
    - If not automatically logged in, proceed to login
    - **📸 Screenshot:** Account dashboard after successful registration

13. Verify account information:
    - Check that username/email is displayed
    - Verify account balance shows 0 CLP
    - Check account status
    - **📸 Screenshot:** Account overview with all details

**Expected Results:**
- ✅ Registration form loads correctly with all fields
- ✅ All fields accept valid Chilean data
- ✅ RUT validation works properly
- ✅ Email format validation works
- ✅ Password requirements are enforced (if any)
- ✅ All mandatory checkboxes must be accepted
- ✅ Registration processes successfully
- ✅ Confirmation message displayed
- ✅ Verification email sent (if required)
- ✅ Email verification successful (if required)
- ✅ SMS verification successful (if required)
- ✅ User account is created and active
- ✅ User can access their account dashboard
- ✅ Account balance displays correctly (0 CLP)

**Post-Test:**
- **Record:** Email used for registration
- **Record:** Mobile phone number used
- **Record:** RUT number used
- **Record:** Username/account ID assigned
- **Record:** Verification method used (email, SMS, both)
- **Record:** Any welcome bonus automatically credited

---

## 2. LOGIN TEST SCENARIO

### TC-LOG-001: User Login (Success Scenario)

**Objective:** Successfully login to an existing Rojabet Chile account with valid credentials

**Preconditions:**
- User account must already be registered (TC-REG-001 completed)
- Email/phone verification completed (if required)
- Account is active and not blocked
- You have correct login credentials

**Test Steps:**

1. Navigate to https://rojabet.com/
   - **📸 Screenshot:** Homepage

2. Locate and click the Login button
   - Look for "Iniciar Sesión", "Login", "Ingresar" in header/top right
   - **📸 Screenshot:** Login button location

3. Login form/modal should appear
   - **📸 Screenshot:** Login form displayed

4. Review login form elements:
   - Email or Username field
   - Password field
   - Show/Hide password option (if available)
   - "Forgot password?" or "¿Olvidaste tu contraseña?" link
   - Login button
   - Social login options (if available)
   - Link to registration (if you don't have account)
   - **📸 Screenshot:** Complete login form interface

5. Enter your registered email/username:
   - Use credentials from TC-REG-001
   - **📸 Screenshot:** Email/username entered

6. Enter your password:
   - Password should be masked by default
   - **📸 Screenshot:** Password entered (masked)

7. (Optional) Test password visibility toggle if available:
   - Click show/hide icon
   - Verify password becomes visible/hidden
   - **📸 Screenshot:** Password visibility toggle (if tested)

8. Click the Login button
   - **📸 Screenshot:** After clicking Login

9. Wait for authentication to complete:
   - **📸 Screenshot:** Processing/loading (if visible)

10. Verify successful login:
    - Login form closes or you're redirected
    - Account dashboard or homepage displays in logged-in state
    - **📸 Screenshot:** Successful login - dashboard/homepage

11. Verify logged-in indicators:
    - Username or email displayed in header
    - Account balance visible (in CLP)
    - Account menu/icon accessible
    - Logout option available
    - **📸 Screenshot:** Header showing logged-in state

12. Access account menu:
    - Click on username/account icon
    - Verify dropdown menu with options:
      - My Account / Mi Cuenta
      - Balance / Saldo
      - Deposit / Depositar
      - Withdrawal / Retirar
      - Transaction History / Historial
      - Settings / Configuración
      - Logout / Cerrar Sesión
    - **📸 Screenshot:** Account menu expanded

13. Navigate to account dashboard:
    - Click on "My Account" or similar
    - **📸 Screenshot:** Full account dashboard

14. Verify dashboard information:
    - Current balance in CLP
    - Account details
    - Recent activity or transactions
    - Quick access buttons (deposit, withdrawal)
    - Promotions or bonus information
    - Account verification status
    - **📸 Screenshot:** Complete dashboard view

**Expected Results:**
- ✅ Login form displays correctly
- ✅ Email/username field accepts input
- ✅ Password field masks input
- ✅ Password visibility toggle works (if available)
- ✅ "Forgot password?" link is visible and functional
- ✅ Login button is clickable with credentials entered
- ✅ Authentication processes successfully
- ✅ No error messages displayed
- ✅ User redirected to logged-in state
- ✅ Username displayed in header
- ✅ Account balance visible and accurate
- ✅ Account menu accessible with all options
- ✅ All account features accessible
- ✅ Session persists (stays logged in on page refresh)

**Post-Test:**
- **Record:** Login credentials used
- **Record:** Username displayed
- **Record:** Current account balance
- **Record:** Account verification status
- **Record:** Any active bonuses or promotions

---

## 3. KYC VERIFICATION (COMPLETE WHEN REQUIRED)

### TC-KYC-001: KYC Document Verification

**Objective:** Complete KYC (Know Your Customer) verification when required

**IMPORTANT NOTES:**
- KYC may be required at different stages:
  - After registration
  - Before first deposit
  - Before withdrawal
  - After reaching certain limits
- Complete this test whenever the platform prompts for KYC
- If KYC is not immediately required, skip and return when prompted

**Preconditions:**
- User is logged in
- Platform is requesting KYC verification
- You have required documents ready (valid and current)

**Required Documents (Typical):**
- Chilean National ID (Cédula de Identidad) - Front
- Chilean National ID (Cédula de Identidad) - Back
- Proof of Address (utility bill or bank statement less than 3 months old)
- Selfie with ID (may be required)

**Test Steps:**

1. When prompted for KYC, locate the verification section:
   - May appear as popup, banner, or in account settings
   - Look for "Verificar Cuenta", "Verificación", "KYC"
   - **📸 Screenshot:** KYC prompt/notification

2. Click to start verification process:
   - **📸 Screenshot:** KYC upload page

3. Review document requirements:
   - **📸 Screenshot:** Document requirements listed

4. Upload Front of Chilean ID:
   - Click upload button for front ID
   - Select clear, high-quality image (JPG, PNG, PDF under 5MB)
   - **📸 Screenshot:** Front ID uploaded

5. Upload Back of Chilean ID:
   - Click upload button for back ID
   - Select image file
   - **📸 Screenshot:** Back ID uploaded

6. Upload Proof of Address:
   - Click upload button for address proof
   - Select document showing: name, address, recent date (within 3 months)
   - **📸 Screenshot:** Address proof uploaded

7. Upload Selfie with ID (if required):
   - Take or upload selfie holding ID
   - Ensure face and ID are clearly visible
   - **📸 Screenshot:** Selfie uploaded

8. Review all uploaded documents:
   - Verify all required documents uploaded
   - Check thumbnails/previews are visible
   - **📸 Screenshot:** All documents ready to submit

9. Click Submit button:
   - **📸 Screenshot:** Submission confirmation

10. Note verification status:
    - Status should show "Under Review", "Pending", or similar
    - **📸 Screenshot:** KYC status after submission

11. Check confirmation email:
    - Email confirming documents received
    - **📸 Screenshot:** Email confirmation

12. Wait for review completion (typically 24-48 hours):
    - Check periodically or wait for email notification
    - **📸 Screenshot:** Approval email when received

13. Verify KYC approval in account:
    - Login and check verification status
    - Should show "Verified", "Verificado", or verification badge
    - **📸 Screenshot:** Account showing verified status

**Expected Results:**
- ✅ All documents upload successfully
- ✅ Accepted file formats work correctly
- ✅ File size limits are appropriate
- ✅ Submission confirmed
- ✅ Confirmation email received
- ✅ Status changes to "Under Review"
- ✅ Within 24-48 hours: KYC approved
- ✅ Approval email received
- ✅ Account status shows "Verified"
- ✅ Full platform functionality unlocked
- ✅ Can proceed with deposits and withdrawals

**Post-Test:**
- **Record:** Documents submitted
- **Record:** Submission date/time
- **Record:** Verification status
- **Record:** Approval date/time
- **Record:** Time taken for approval
- **Record:** Any new features/limits unlocked

---

## 4. DEPOSIT TEST SCENARIO

### TC-DEP-001: Minimum Deposit

**Objective:** Successfully deposit the minimum allowed amount to the account

**Preconditions:**
- User is logged in
- KYC verification completed (if required for deposits)
- Valid payment method available

**Test Steps:**

1. From account dashboard, locate Deposit button:
   - Look for "Depositar", "Deposit", "Recargar"
   - **📸 Screenshot:** Deposit button location

2. Click Deposit button:
   - **📸 Screenshot:** Deposit page/modal

3. Review available deposit methods:
   - Credit/Debit Cards (Visa, Mastercard)
   - Bank Transfer
   - Digital Wallets (Mercado Pago, MACH, etc.)
   - Other local Chilean payment methods
   - **📸 Screenshot:** All available payment methods

4. Select your preferred payment method:
   - Click on the method you will use
   - **📸 Screenshot:** Selected payment method

5. Review deposit limits:
   - Note minimum deposit amount
   - Note maximum deposit amount
   - **📸 Screenshot:** Deposit limits displayed

6. Enter the MINIMUM deposit amount:
   - Enter exact minimum allowed (e.g., 5,000 CLP)
   - **📸 Screenshot:** Minimum amount entered

7. Review any fees or charges:
   - Check if processing fees shown
   - **📸 Screenshot:** Fee breakdown (if any)

8. Review welcome bonus eligibility (if first deposit):
   - Check if welcome bonus applies
   - Review bonus terms if applicable
   - **📸 Screenshot:** Bonus information (if applicable)

9. Enter payment details:
   - For cards: card number, expiry, CVV, name
   - For bank: follow instructions
   - For wallets: may redirect to app/website
   - **📸 Screenshot:** Payment details entry (mask sensitive info)

10. Review transaction summary:
    - Deposit amount
    - Payment method
    - Any fees
    - Bonus (if applicable)
    - Total to be charged
    - **📸 Screenshot:** Transaction summary

11. Click Confirm/Process Payment:
    - **📸 Screenshot:** Confirmation button

12. Complete additional verification:
    - 3D Secure for cards (enter OTP if prompted)
    - Wallet authentication
    - **📸 Screenshot:** Additional authentication (if applicable)

13. Wait for transaction processing:
    - **📸 Screenshot:** Processing screen

14. Verify deposit confirmation:
    - Success message displayed
    - Transaction ID/reference number provided
    - **📸 Screenshot:** Deposit success confirmation

15. Check account balance update:
    - Balance should increase by deposit amount (plus bonus if applicable)
    - **📸 Screenshot:** Updated account balance

16. Verify welcome bonus credited (if first deposit):
    - Check if bonus amount added
    - Review bonus terms/wagering requirements
    - **📸 Screenshot:** Bonus balance (if applicable)

17. Check transaction history:
    - Navigate to transaction history
    - Locate deposit transaction
    - Verify: date, time, amount, method, status (completed)
    - **📸 Screenshot:** Deposit in transaction history

18. Check email confirmation:
    - Email confirming deposit
    - **📸 Screenshot:** Deposit confirmation email

**Expected Results:**
- ✅ Deposit page loads correctly
- ✅ All payment methods displayed
- ✅ Minimum/maximum limits clearly shown
- ✅ Minimum amount accepted
- ✅ Payment details form works properly
- ✅ Payment processed successfully
- ✅ Transaction confirmed with reference number
- ✅ Funds credited immediately (or within stated timeframe)
- ✅ Account balance updated correctly
- ✅ Welcome bonus credited if applicable
- ✅ Transaction appears in history
- ✅ Confirmation email received

**Post-Test:**
- **Record:** Deposit amount
- **Record:** Payment method used
- **Record:** Transaction ID/reference
- **Record:** Processing fees (if any)
- **Record:** Welcome bonus received (if applicable)
- **Record:** New account balance
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

1. From dashboard, navigate to Casino section:
   - Look for "Casino", "Slots", "Juegos", "Tragamonedas"
   - **📸 Screenshot:** Casino section button

2. Casino lobby should load:
   - **📸 Screenshot:** Casino game lobby

3. Browse available games:
   - Review slot machines available
   - Note providers: Pragmatic Play, Evolution Gaming, etc.
   - **📸 Screenshot:** Game selection/categories

4. Select a slot machine game:
   - Choose any slot game that interests you
   - **📸 Screenshot:** Selected slot game

5. Click to launch the game:
   - Game may open in same window or new window
   - Wait for game to load completely
   - **📸 Screenshot:** Game loading

6. Review game interface when loaded:
   - Game screen with reels
   - Spin button
   - Bet amount controls
   - Balance display
   - Info/Paytable button
   - Settings/Sound controls
   - **📸 Screenshot:** Fully loaded game interface

7. Verify balance in game:
   - Balance should match account balance
   - Should display in CLP
   - **📸 Screenshot:** Balance in game

8. Set bet amount:
   - Locate bet controls (+/- buttons or bet selector)
   - Start with minimum bet or adjust as preferred
   - **📸 Screenshot:** Bet amount selected

9. Review bet configuration:
   - Bet per line (if applicable)
   - Number of lines (if applicable)
   - Total bet amount
   - **📸 Screenshot:** Bet configuration

10. Place first bet - click Spin button:
    - **📸 Screenshot:** Spin button / Game spinning

11. Wait for spin to complete:
    - **📸 Screenshot:** Spin result (win or lose)

12. Check result and balance:
    - Note if you won or lost
    - Verify balance updated
    - **📸 Screenshot:** Balance after first spin

13. Place additional bets (minimum 5 total spins):
    - Spin 2: **📸 Screenshot:** Result
    - Spin 3: **📸 Screenshot:** Result
    - Spin 4: **📸 Screenshot:** Result
    - Spin 5: **📸 Screenshot:** Result

14. Check game history (if available):
    - **📸 Screenshot:** Game history in slot

15. Note final balance after all spins:
    - **📸 Screenshot:** Final balance in game

16. Exit game:
    - Click back/exit/close button
    - Return to casino lobby or main platform
    - **📸 Screenshot:** Exiting game

17. Verify account balance on platform:
    - Balance should reflect all bets placed
    - **📸 Screenshot:** Account balance after gaming

18. Check transaction history:
    - Navigate to account history
    - Locate casino game transactions
    - Verify all bets recorded correctly
    - **📸 Screenshot:** Casino bets in history

**Expected Results:**
- ✅ Casino section accessible
- ✅ Game lobby loads with games
- ✅ Slot game launches properly
- ✅ Game interface displays correctly
- ✅ Balance syncs with account
- ✅ Bet controls work properly
- ✅ Spin button responsive
- ✅ Game plays smoothly without errors
- ✅ Results display clearly
- ✅ Balance updates in real-time
- ✅ Wins credited correctly (if any)
- ✅ All bets recorded in history
- ✅ Can exit game successfully
- ✅ Final balance accurate on platform

**Post-Test:**
- **Record:** Slot game name/provider
- **Record:** Starting balance
- **Record:** Bet amount per spin
- **Record:** Number of spins played
- **Record:** Total amount wagered
- **Record:** Any wins received
- **Record:** Final balance
- **Record:** Net profit/loss

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

**IMPORTANT:** KYC must be completed before withdrawal. Complete TC-KYC-001 first if needed.

**Test Steps:**

1. From dashboard, locate Withdrawal button:
   - Look for "Retirar", "Withdrawal", "Retiro"
   - **📸 Screenshot:** Withdrawal button location

2. Click Withdrawal button:
   - **📸 Screenshot:** Withdrawal page

3. Review withdrawal requirements:
   - KYC status must be verified
   - Minimum withdrawal amount
   - Any pending wagering requirements
   - **📸 Screenshot:** Requirements displayed

4. Review available withdrawal methods:
   - Bank Transfer
   - Digital Wallets
   - Other available methods
   - **📸 Screenshot:** Available withdrawal methods

5. Select Bank Transfer (most common):
   - **📸 Screenshot:** Selected method

6. Enter or verify bank account details:
   - **If first withdrawal:**
     - Bank name
     - Account type (Cuenta Corriente/Cuenta Vista)
     - Account number
     - Account holder name (must match registered name)
     - RUT
   - **If previously saved:** Verify details correct
   - **📸 Screenshot:** Bank details (mask account number)

7. Review withdrawal limits:
   - Note minimum withdrawal amount
   - Note maximum withdrawal amount
   - **📸 Screenshot:** Withdrawal limits

8. Enter withdrawal amount:
   - Amount within limits and available balance
   - **📸 Screenshot:** Withdrawal amount entered

9. Review fees and processing time:
   - Check for withdrawal fees
   - Review estimated processing time
   - **📸 Screenshot:** Fee and processing info

10. Review withdrawal summary:
    - Amount to withdraw
    - Destination (bank account)
    - Fees (if any)
    - Net amount to receive
    - Estimated time
    - **📸 Screenshot:** Withdrawal summary

11. Complete additional verification (if prompted):
    - 2FA code (SMS/Email)
    - Security questions
    - **📸 Screenshot:** Verification step

12. Click Confirm/Submit Withdrawal:
    - **📸 Screenshot:** Confirmation button

13. Wait for processing:
    - **📸 Screenshot:** Processing screen

14. Verify withdrawal submission:
    - Success message
    - Transaction ID/reference
    - Status: "Pending" or "Processing"
    - **📸 Screenshot:** Withdrawal confirmation

15. Check account balance:
    - Amount deducted or marked as pending
    - **📸 Screenshot:** Updated balance

16. Check transaction history:
    - Locate withdrawal transaction
    - Verify: date, time, amount, method, status
    - **📸 Screenshot:** Withdrawal in history

17. Check confirmation email:
    - Email confirming withdrawal request
    - **📸 Screenshot:** Withdrawal email

18. Monitor withdrawal status (1-5 business days):
    - Check platform for status updates
    - **📸 Screenshot:** Status updates

19. Verify funds received in bank:
    - Check bank account after processing period
    - Confirm funds arrived
    - **📸 Screenshot:** Bank statement (mask sensitive info)

20. Verify final status in platform:
    - Login to Rojabet
    - Check transaction history
    - Status should be "Completed" or "Completado"
    - **📸 Screenshot:** Final completed status

**Expected Results:**
- ✅ Withdrawal page accessible
- ✅ KYC verified status confirmed
- ✅ Withdrawal methods displayed
- ✅ Bank details can be entered/saved
- ✅ Withdrawal limits clearly shown
- ✅ Amount validation works
- ✅ Withdrawal submitted successfully
- ✅ Confirmation and transaction ID provided
- ✅ Balance updated (amount reserved)
- ✅ Transaction in history with "Pending" status
- ✅ Confirmation email received
- ✅ Within 1-5 business days: funds arrive in bank
- ✅ Transaction status updated to "Completed"
- ✅ Amount received matches withdrawal (minus fees)

**Post-Test:**
- **Record:** Withdrawal amount
- **Record:** Withdrawal method
- **Record:** Transaction ID/reference
- **Record:** Bank account used (last 4 digits)
- **Record:** Stated processing time
- **Record:** Actual processing time
- **Record:** Fees charged (if any)
- **Record:** Final amount received
- **Record:** Any issues or delays

---

## 7. END-TO-END TEST SCENARIO

### TC-E2E-001: Complete User Journey

**Objective:** Execute complete user journey from registration through withdrawal

**This comprehensive test combines all previous test cases in sequence.**

**Test Flow:**

1. ✅ **REGISTRATION** (TC-REG-001)
   - Register new user account
   - Complete email/SMS verification
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
   - Note any welcome bonus
   - **📸 Screenshots:** As per TC-DEP-001

5. ⚠️ **KYC VERIFICATION** (TC-KYC-001 - If Required)
   - If KYC not completed earlier and now required, complete it
   - **📸 Screenshots:** As per TC-KYC-001 (when completed)

6. ✅ **PLACE BETS** (TC-BET-001)
   - Play casino slot games
   - Place multiple bets (minimum 5 spins)
   - **📸 Screenshots:** As per TC-BET-001

7. ⚠️ **KYC VERIFICATION** (TC-KYC-001 - If Required)
   - If KYC still not done and required before withdrawal, complete now
   - **📸 Screenshots:** As per TC-KYC-001 (when completed)

8. ✅ **WITHDRAWAL** (TC-WDR-001)
   - Withdraw remaining funds
   - Verify withdrawal processed
   - Confirm funds received in bank
   - **📸 Screenshots:** As per TC-WDR-001

**Expected Results:**
- ✅ All steps complete successfully in sequence
- ✅ Smooth transitions between functions
- ✅ KYC completed at required stage
- ✅ All notifications received
- ✅ All transactions recorded accurately
- ✅ Balances remain accurate throughout
- ✅ Complete user lifecycle verified
- ✅ No blocking issues encountered
- ✅ Platform performs consistently

**Post-Test Documentation:**
- **Summary Report:** Complete journey summary
- **Screenshots:** All screenshots organized chronologically
- **Issues:** Any issues encountered (if any)
- **Timing:** Total time for complete journey
- **Notes:** Observations and recommendations

---

## Test Execution Checklist

### Before Starting Tests:
- [ ] Clear browser cache and cookies
- [ ] Prepare valid Chilean personal data (RUT, phone, address)
- [ ] Have valid ID documents ready (for KYC)
- [ ] Have payment method ready (card, wallet, etc.)
- [ ] Have bank account details ready (for withdrawal)
- [ ] Create folder structure for screenshots
- [ ] Ensure stable internet connection
- [ ] Note current date/time for test session

### During Testing:
- [ ] Take screenshot at EVERY step
- [ ] Name screenshots clearly and consistently
- [ ] Record all transaction IDs/references
- [ ] Note exact times for all actions
- [ ] Document any unexpected behavior
- [ ] Save all email confirmations
- [ ] Save all SMS confirmations

### After Testing:
- [ ] Organize all screenshots by test case
- [ ] Complete test results documentation
- [ ] Calculate total time for each test
- [ ] Document any deviations from expected results
- [ ] Prepare summary report
- [ ] Archive all test materials

---

## Test Results Template

For each test case, document:

**Test Case ID:** [TC-XXX-001]
**Test Case Name:** [Test Name]
**Date Executed:** [YYYY-MM-DD]
**Tester Name:** [Your Name]
**Browser/Device:** [Chrome/Firefox/Safari/Mobile]
**Test Result:** [PASS / FAIL / BLOCKED]

**Execution Details:**
- Start Time: [HH:MM]
- End Time: [HH:MM]
- Duration: [X minutes]

**Test Data Used:**
- Email: [email used]
- Phone: [phone used]
- Amounts: [deposit/withdrawal amounts]
- Transaction IDs: [list all IDs]

**Screenshots Captured:** [Number of screenshots]
**Screenshots Location:** [Folder path or reference]

**Actual Results:**
- [Describe what actually happened during test execution]

**Comparison to Expected Results:**
- [PASS] All expected results achieved
- OR
- [FAIL] List any deviations from expected results

**Issues Encountered:**
- [None]
- OR
- [List any problems, errors, delays, unexpected behavior]

**Additional Notes:**
- [Any observations, recommendations, or comments]

---

## Screenshot Organization

Suggested folder structure:

```
Rojabet_Testing_[YYYY-MM-DD]/
├── TC-REG-001_Registration/
│   ├── Step-01-Homepage.png
│   ├── Step-02-Registration-Button.png
│   ├── Step-03-Registration-Form.png
│   └── ...
├── TC-LOG-001_Login/
│   ├── Step-01-Homepage.png
│   ├── Step-02-Login-Button.png
│   └── ...
├── TC-KYC-001_Verification/
│   ├── Step-01-KYC-Prompt.png
│   └── ...
├── TC-DEP-001_Deposit/
│   ├── Step-01-Deposit-Button.png
│   └── ...
├── TC-BET-001_Casino_Betting/
│   ├── Step-01-Casino-Section.png
│   └── ...
├── TC-WDR-001_Withdrawal/
│   ├── Step-01-Withdrawal-Button.png
│   └── ...
├── TC-E2E-001_End_to_End/
│   └── [Organized by substeps]
└── Test_Summary_Report.pdf
```

---

## Final Deliverables

After completing all tests, provide:

1. **Screenshot Package**
   - All screenshots organized by test case
   - Clear naming convention followed
   - Organized in folder structure

2. **Test Results Summary**
   - Document with results for each test case
   - Pass/Fail status for each test
   - Summary statistics

3. **Transaction Log**
   - List of all transactions
   - Transaction IDs and amounts
   - Dates and times
   - Status of each transaction

4. **Issues Log**
   - Any problems encountered
   - Steps to reproduce issues
   - Screenshots of issues
   - Severity and priority

5. **Timing Report**
   - Duration for each test case
   - Total testing time
   - Any delays or wait times

6. **Test Summary Report**
   - Executive summary
   - Overall pass/fail rate
   - Key findings
   - Recommendations (if any)

---

## Important Reminders

- 📸 **Screenshot EVERYTHING** - Cannot emphasize this enough
- ✅ **Complete KYC whenever required** - Don't skip this step
- 💰 **Use minimum deposit amount** - Cost-effective testing
- 🎰 **Test casino slots** - Easier than sports betting for functional testing
- 📝 **Document all transaction IDs** - Critical for tracking
- 📧 **Keep all email confirmations** - Important proof of transactions
- ⏱️ **Record all timing** - Helps identify performance issues
- ✔️ **Focus on SUCCESS scenarios** - This document is for positive testing only
- 🔍 **Be thorough** - Don't rush, complete every step
- 💾 **Save everything** - Better to have too much documentation than too little

---

## Platform-Specific Notes for Rojabet

**Welcome Bonus:**
- Rojabet offers welcome bonuses for first deposits
- Check if bonus is automatically applied or needs activation
- Review wagering requirements before attempting withdrawal
- Document bonus terms and conditions

**Chilean Features:**
- Platform is specifically for Chilean market
- All transactions in CLP (Chilean Pesos)
- RUT required for registration and verification
- Chilean bank accounts for withdrawals
- Local payment methods available

**Game Providers:**
- Pragmatic Play
- Evolution Gaming
- CT Interactive
- Other providers as available

**Sports Betting:**
- If testing sports betting instead of slots, adapt TC-BET-001 accordingly
- Focus on pre-match betting for easier testing
- Document odds, stake, potential win, and actual result

**Additional Features:**
- Live Casino (if testing, document dealer interaction)
- Virtual Sports
- "La Polla" (Chilean lottery-style game)
- Live Streaming (if available during test)

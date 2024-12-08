# CRUD Operation Manual Testing Checklist

| **Test Area**       | **Test Case**                                                                                  
|----------------------|-----------------------------------------------------------------------------------------------
| **Input Validation** | Ensure all required fields are filled.                                                       
|                      | Test with invalid inputs (e.g., letters in numeric fields, special characters).               
|                      | Verify character limits or value boundaries for fields.                                       
| **API Request & Response** | Test successful API responses (e.g., status `201` for POST, `200` for PUT).             
|                      | Confirm data is saved or updated correctly on the server.                                     
|                      | Test with missing or invalid data and ensure appropriate error messages.                      
|                      | Simulate server errors and ensure fallback behavior works (e.g., "Server unavailable").       
| **UI Behavior**      | Verify loading states during the operation (e.g., spinner or message).                       
|                      | Check for success feedback (e.g., "Data saved successfully").                                 
|                      | Ensure error feedback is displayed for failures (e.g., "Invalid data").                       
|                      | Verify the form resets or retains values as expected after submission.                        
| **Data Integrity**   | Check the database/backend for consistent data after the operation.                           
|                      | Verify updated data reflects correctly in all related views or components.                    
| **Edge Cases**       | Submit empty data and ensure validation works.                                                
|                      | Test with large inputs, such as big files or long strings.                                    
|                      | Test with special characters or unexpected input formats.                                    
| **Error Scenarios**  | Test with expired or invalid authentication tokens.                                           
|                      | Test with disconnected internet or failing server.                                           
|                      | Simulate rate-limiting or throttling if applicable.                                           
| **Undo/Redo**        | If undo/redo is supported, verify previous state is restored correctly.                       
| **Cross-Browser**    | Test the operation on different browsers (Chrome, Firefox, Edge, Safari).                     
| **Responsiveness**   | Check the UI behavior on different devices (mobile, tablet, desktop).                         
| **Tools**            | Use Postman or Insomnia to test API requests and responses.                                  
|                      | Use browser DevTools to monitor network requests and check for console errors.               
|                      | Verify logs in the backend for debugging or validation.                                       

---

## **How to Use This Checklist**

1. Review the test cases before starting your manual testing session.
2. Add any additional scenarios specific to your application.

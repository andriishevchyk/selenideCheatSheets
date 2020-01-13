# Selenide Cheat Sheets

1. `$x(format("//span[contains(text(), '%s')]",  comment))` -> `$$("span").find(exactText(comment));`

2. `ancestor::tr` -> `closest("tr")`

3. `$x("//button[starts-with(@id, 'remove')]")` -> `$("button[id*='remove']")`

4. `$x("//td[contains(@class,'ui-datepicker-today')]")` - > `$("td.ui-datepicker-today")`

5. `$x("//textarea[@id='sl-comment']")` -> `$("#sl-comment")`

6. `$("button[style="display: block;"])` -> `$$("button").find(attribute("display", "block"))`

7. `$("textarea[class*=form-control]")` -> `$("textarea.form-control")`

8. `$(By.id("SimpleSearchInput"))` -> `$("#SimpleSearchInput");`

9. `$(By.className("loader-box"));` -> `$(".loader-box");`

# Asserts
---

 `assertThat(employeeAttendance.getSuperiorMessage().getText())
                   .as("Superior comment when rejecting time off request")
                   .isEqualTo("Need more information");`
            
   ->          
               
`superiorMessage.shouldHave(exactText("Need more information"));`

   ---
   
   
   



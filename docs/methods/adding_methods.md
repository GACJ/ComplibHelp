# Adding Methods
Complib gives registered users the ability to create custom methods.

To get started, click on **Create new > New method** in the navbar or dropdown menu:

![Navbar Create New](../img/navbar_create_new.png){ width="300" }
![Dropdown Menu Create New](../img/dropdown_menu_create_new.png){ width="300" }

## The add method page
![Add Method Page](../img/add_method_page.png){ width="500"}

The add method page has a number of fields which allow you to specify certain properties of your custom method. These are:

Name (optional)
:   The desired name for your custom method. This will be used by Complib to generate the method's full title, which consists of its name plus its classification and stage.

!!! note
    Complib automatically appends the method's classification and stage to its name. As such, you should not add classification- or stage-specific words such as `Treble Bob` or `Caters` to the name field.

!!! warning
    While the name field is optional, it is strongly recommended that you give every custom method a name. This will allow you to search for it more easily later.

Stage (required)
:   The stage at which the method is to be rung. Complib supports methods on up to twenty-eight bells.

Place Notation (required)
:   The method's place notation. This can be specified in either full or condensed form. When verifying the method, Complib will automatically condense the place notation as much as possible. To learn how to use place notation, see [Place notation](place_notation.md).

Division Ends (optional)
:   For methods requiring divisions, specifies the rows at the ends of each division. If the method has multiple divisions per lead, the corresponding division end rows should be separated with a colon (e.g., `2:8`).

Notes (optional)
:   Specifies a message to be displayed in the **Library Details** tab of the custom method's page. This is a good place to put any important information about the method which you may want to keep to hand.

## Validating methods, method errors & warnings
Complib will automatically attempt to validate a custom method as soon as its place notation is specified. If the provided place notation is valid, the custom method's full name, diagram and properties will be generated and displayed. Clicking the `Validate` button will force a re-validation.

If the custom method is successfully validated, clicking the `Save` button will save the custom method as a **private method**.

### Method errors

![Method error message](../img/method_error_message.png)

If Complib encounters a problem when attempting to validate a custom method, an error message will be displayed. **All errors must be cleared before a custom method can be saved.**

There are a number of different error types:

!!! error "Error: Place notation `_` is invalid for stage..."

The identified element of place notation is not valid for the specified stage. Usually this means that the place specified in the place notation element does not exist at this stage. For example, attempting to validate the element `18` at stages lower than `Major` will generate this error.

!!! error "Error: Method title already used..."

The title generated for the custom method conflicts with the title of an already existing method. The custom method's name must be altered so that the generated title is unique.

!!! error "Error: Method place notation already exists as..."

The specified place notation is identical to that of an already existing method. The custom method's place notation must be altered so that it is unique.

!!! error "Error: Method cannot be classified... "

Complib cannot parse the specified place notation. This happens when the specified place notation does not conform to one of the accepted Method XML formats, or is empty. See [Place notation](place_notation.md) to learn more about the place notations that Complib can accept.

!!! error "Error: Division Ends must be positive and less than the lead length."

The specified division ends exceed the bounds of the method's lead. The division ends must be rows within the lead length of the method as determined from its place notation.

!!! error "Error: Division Ends must be unique."

For custom methods with multiple divisions, two or more of the specified division ends are identical. All division ends must be unique rows within the method's lead.

### Warnings and other messages
If method validation is successful, Complib may display a number of warnings and other messages.


## Private and public methods

### Sharing private methods

## Editing and deleting methods

## Linking Bellboard performances


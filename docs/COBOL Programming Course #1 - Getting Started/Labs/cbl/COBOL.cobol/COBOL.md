```markdown
## Documentation

This COBOL program demonstrates basic file operations, looping, and date/time handling. It opens an output file (PRT-LINE), writes a sequence of numbers to it, then opens a second output file (PRT-DONE) and writes a completion record containing the current date, time, and a comment.

## Sections/Paragraphs

### A000-START

This section initializes the program. It opens the PRT-LINE output file and then calls the A000-COUNT paragraph 10 times. Finally, it calls the A000-DONE paragraph for final processing and closes the PRT-LINE file before ending the program.

### A000-COUNT

This section increments a counter (PGM-COUNT) and writes its current value to the PRT-LINE file.  The `DISPLAY` statement is commented out.

### A000-DONE

This section handles final processing. It opens the PRT-DONE output file, retrieves the current date and time, formats them, and writes them to the PRT-DONE file along with a predefined comment. Lastly, it closes the PRT-DONE file.
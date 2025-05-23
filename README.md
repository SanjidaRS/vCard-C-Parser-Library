# vCard C Parser Library

This project is a modular, memory-safe C library designed to parse, validate, and serialize vCard (`.vcf`) files, conforming to the [RFC 6350](https://datatracker.ietf.org/doc/html/rfc6350) standard. It provides a clean and extensible API suitable for integration into larger systems like contact managers or front-end applications built in other languages (e.g., Python GUIs).

## 🔧 Key Features

- **vCard Parsing**  
  Parses `.vcf` files into structured in-memory representations using dynamic data structures.

- **Data Serialization**  
  Converts structured card data back into vCard-compliant file output.

- **Validation Engine**  
  Validates card structure and content integrity, including constraints like required properties, correct formats, and valid cardinality.

- **Error Management**  
  Detailed error reporting using specific codes (`INV_FILE`, `INV_CARD`, `INV_PROP`, `INV_DT`, etc.) with human-readable messages.

- **Memory Safety**  
  Full support for dynamic memory management with rigorous deallocation to prevent memory leaks.

- **Line Unfolding**  
  Handles standard line folding/unfolding as per vCard spec to ensure compatibility.

## 🗂 Project Structure
vcard-parser/
│
├── bin/ # Compiled shared library (libvcparser.so)
├── include/ # Header files for helper functions
├── src/ # Source files (VCParser.c, VCHelpers.c, LinkedListAPI.c)
├── Makefile # Build automation: make parser, make clean


## ⚙️ Technologies Used

- **C (GCC)**
- **Linked List API**
- **Valgrind** (for memory checks)
- **Makefile Build System**
- **RFC 6350 Compliant Design**

## 🧪 Example Use Cases

- Backend logic for contact management systems
- Integration with user-facing apps for viewing and editing contacts
- Educational tools for teaching structured file parsing and serialization

## ✅ How to Build

Ensure you have `gcc` and `make` installed. Then run:

```bash
make parser     # Builds libvcparser.so in the /bin directory
make clean      # Removes object and shared library files

📌 Future Enhancements
Python wrapper using ctypes for GUI integration

Extended validation for international vCard properties

Support for contact search and filtering via CLI

👤 Author
Sanjida Rahman Supti
Bachelor of Computing (Honours), Computer Science
University of Guelph

🌐 Portfolio

🐙 GitHub

💼 LinkedIn

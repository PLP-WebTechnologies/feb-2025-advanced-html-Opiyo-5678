# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced HTML5 Elements and Forms</title>
</head>
<body>
    <header>
        <h1>Advanced HTML5 Elements and Forms</h1>
        <nav>
            <ul>
                <li><a href="#list-section">Ordered List</a></li>
                <li><a href="#image-section">Image</a></li>
                <li><a href="#table-section">Contacts Table</a></li>
                <li><a href="#form-section">Registration Form</a></li>
                <li><a href="#multimedia-section">Multimedia</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- Ordered List with Roman Numerals -->
        <section id="list-section">
            <h2>HTML5 Main Features</h2>
            <ol type="I">
                <li>Semantic Elements</li>
                <li>Form Enhancements</li>
                <li>Multimedia Support</li>
                <li>Canvas and SVG</li>
                <li>Local Storage</li>
                <li>Responsive Design Support</li>
            </ol>
        </section>

        <!-- External Image from Pexels -->
        <section id="image-section">
            <h2>Featured Image</h2>
            <figure>
                <img src="https://images.pexels.com/photos/1089438/pexels-photo-1089438.jpeg" 
                     alt="Computer with code on screen"
                     width="600"
                     height="400">
                <figcaption>Modern web development with HTML5</figcaption>
            </figure>
        </section>

        <!-- Table of Contacts -->
        <section id="table-section">
            <h2>Contact Directory</h2>
            <table border="1">
                <caption>Our Team Members</caption>
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Address</th>
                        <th>Mobile</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>John Smith</td>
                        <td>123 Main St, Boston, MA</td>
                        <td>555-123-4567</td>
                        <td>john.smith@example.com</td>
                    </tr>
                    <tr>
                        <td>Sarah Johnson</td>
                        <td>456 Oak Ave, Chicago, IL</td>
                        <td>555-987-6543</td>
                        <td>sarah.j@example.com</td>
                    </tr>
                    <tr>
                        <td>Michael Brown</td>
                        <td>789 Pine Rd, Seattle, WA</td>
                        <td>555-456-7890</td>
                        <td>m.brown@example.com</td>
                    </tr>
                    <tr>
                        <td>Emma Davis</td>
                        <td>321 Cedar Ln, Austin, TX</td>
                        <td>555-234-5678</td>
                        <td>emma.d@example.com</td>
                    </tr>
                    <tr>
                        <td>James Wilson</td>
                        <td>654 Maple Dr, Denver, CO</td>
                        <td>555-876-5432</td>
                        <td>j.wilson@example.com</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Registration Form -->
        <section id="form-section">
            <h2>Registration Form</h2>
            <form action="/submit-registration" method="post">
                <!-- Name Field -->
                <div>
                    <label for="fullName">Full Name:</label>
                    <input type="text" id="fullName" name="fullName" placeholder="Enter your full name" required>
                </div>

                <!-- Email Field -->
                <div>
                    <label for="email">Email Address:</label>
                    <input type="email" id="email" name="email" placeholder="your.email@example.com" required>
                </div>

                <!-- Password Field -->
                <div>
                    <label for="password">Password:</label>
                    <input type="password" id="password" name="password" 
                           placeholder="Create a password" 
                           minlength="8" 
                           pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}" 
                           title="Must contain at least one number, one uppercase and lowercase letter, and at least 8 characters"
                           required>
                    <small>Password must be at least 8 characters with numbers, uppercase and lowercase letters</small>
                </div>

                <!-- Date Field -->
                <div>
                    <label for="birthdate">Date of Birth:</label>
                    <input type="date" id="birthdate" name="birthdate" required>
                </div>

                <!-- Dropdown -->
                <div>
                    <label for="country">Country:</label>
                    <select id="country" name="country" required>
                        <option value="">Select your country</option>
                        <option value="us">United States</option>
                        <option value="ca">Canada</option>
                        <option value="uk">United Kingdom</option>
                        <option value="au">Australia</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <!-- Radio Buttons -->
                <div>
                    <fieldset>
                        <legend>Gender:</legend>
                        <input type="radio" id="male" name="gender" value="male">
                        <label for="male">Male</label>
                        
                        <input type="radio" id="female" name="gender" value="female">
                        <label for="female">Female</label>
                        
                        <input type="radio" id="non-binary" name="gender" value="non-binary">
                        <label for="non-binary">Non-binary</label>
                        
                        <input type="radio" id="prefer-not" name="gender" value="prefer-not">
                        <label for="prefer-not">Prefer not to say</label>
                    </fieldset>
                </div>

                <!-- Checkboxes -->
                <div>
                    <fieldset>
                        <legend>Interests (select all that apply):</legend>
                        <input type="checkbox" id="web-dev" name="interests" value="web-dev">
                        <label for="web-dev">Web Development</label>
                        
                        <input type="checkbox" id="mobile-dev" name="interests" value="mobile-dev">
                        <label for="mobile-dev">Mobile Development</label>
                        
                        <input type="checkbox" id="ui-design" name="interests" value="ui-design">
                        <label for="ui-design">UI/UX Design</label>
                        
                        <input type="checkbox" id="data-science" name="interests" value="data-science">
                        <label for="data-science">Data Science</label>
                    </fieldset>
                </div>

                <!-- Terms and Conditions -->
                <div>
                    <input type="checkbox" id="terms" name="terms" required>
                    <label for="terms">I agree to the terms and conditions</label>
                </div>

                <!-- Submit Button -->
                <div>
                    <button type="submit">Register</button>
                    <button type="reset">Clear Form</button>
                </div>
            </form>
        </section>

        <!-- Multimedia Section -->
        <section id="multimedia-section">
            <h2>Multimedia Elements</h2>
            
            <!-- Audio Element -->
            <article>
                <h3>Audio Sample</h3>
                <audio controls>
                    <source src="https://file-examples.com/storage/fe5467a6a763f220c936c50/2017/11/file_example_MP3_700KB.mp3" type="audio/mpeg">
                    Your browser does not support the audio element.
                </audio>
            </article>
            
            <!-- Video Element -->
            <article>
                <h3>Video Sample</h3>
                <video width="400" height="300" controls>
                    <source src="https://file-examples.com/storage/fe5467a6a763f220c936c50/2017/04/file_example_MP4_480_1_5MG.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
            </article>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Advanced HTML5 Example</p>
        <address>
            Contact us at: <a href="mailto:info@example.com">austineopiyo84@gmail.com</a>
        </address>
    </footer>
</body>
</html>

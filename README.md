# Zoology 4th Semester — AI Question Generator

An AI-powered study tool that generates university exam-oriented questions and answers for Zoology 4th Semester students, covering **Immunology** and **Parasitology**.

## Features

✨ **Smart Question Generation**
- Generate custom questions using Claude AI
- Three question types: Short (~20 words), Long (~200 words), Very Long (300-400 words)
- Subject-specific (Immunology, Parasitology, or Both)
- Unit/Chapter filtering for focused study

📚 **Comprehensive Syllabus Coverage**

### Immunology (4 Units)
- **Unit I**: Overview of Immune System
- **Unit II**: Molecules of Immune System
- **Unit III**: Immunodeficiency and Tumor Immunology
- **Unit IV**: Damaging and Defective Immune Response

### Parasitology (4 Units)
- **Unit I**: Introduction to Parasitology
- **Unit II**: Medical Parasitology
- **Unit III**: Veterinary Parasitology
- **Unit IV**: Agricultural Nematology & Acanthocephalans

🎨 **Modern UI/UX**
- Dark theme with gradient accents
- Expandable question cards
- Copy-to-clipboard functionality
- Word count tracking
- Responsive design

## How to Use

1. **Open** `index.html` in your web browser
2. **Select** your subject (Immunology, Parasitology, or Both)
3. **Choose** unit/chapter or select "All Units"
4. **Pick** question types you want (Short, Long, Very Long)
5. **Set** questions per type (1-8)
6. **Click** "Generate Exam Questions"
7. **Paste** your Anthropic API key when prompted (saved locally)
8. **Expand** answers by clicking on question cards
9. **Copy** answers with the copy button

## Requirements

- **Web Browser** (Chrome, Firefox, Safari, Edge)
- **Anthropic API Key** (from [console.anthropic.com](https://console.anthropic.com))

## API Configuration

The tool uses Claude AI to generate questions. You'll need:

1. Get your API key from [Anthropic Console](https://console.anthropic.com)
2. First run: Tool will prompt for API key
3. API key is stored locally in browser storage (not sent to any server)
4. To reset: Clear browser localStorage or reload

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **AI Engine**: Claude 3.5 Sonnet (Anthropic)
- **Fonts**: Playfair Display, Source Serif 4, JetBrains Mono
- **Architecture**: Client-side only (no backend required)

## File Structure

```
Fazil-s-ai/
├── index.html          # Main application file
├── README.md           # This file
└── .gitignore          # Git ignore rules
```

## Features in Detail

### Question Generation
- Exam-oriented questions directly from syllabus
- Structured JSON responses with questions and answers
- Consistent formatting across question types
- Scientific terminology compliance

### UI Components
- **Subject Selector**: Choose study focus
- **Unit Pills**: Quick navigation through syllabus units
- **Question Type Toggles**: Filter by answer length
- **Quantity Control**: Adjust questions per type (1-8)
- **Loading Indicator**: Real-time feedback during generation
- **Question Cards**: Collapsible Q&A with word counts

### Data Management
- Local API key storage
- Session-based question caching
- Copy-to-clipboard for answers
- Timestamp tracking for generated content

## Customization

You can customize the application by editing:

### Syllabus Topics
Modify the `SYLLABUS` object in `<script>` section to:
- Add new units
- Update topics
- Change subject names

### UI Colors
Customize CSS variables in `:root`:
```css
--accent: #3ecf8e;      /* Primary green */
--accent2: #4da6ff;     /* Secondary blue */
--accent3: #f7c948;     /* Tertiary yellow */
```

### Model & Settings
Change in `generateQuestions()` function:
- Model: `claude-3-5-sonnet-20241022`
- Max tokens: `4000`
- Add system prompts as needed

## Troubleshooting

| Issue | Solution |
|-------|----------|
| API Key Prompt Loop | Clear localStorage & reload |
| CORS Errors | Use direct Anthropic endpoint |
| Invalid JSON Response | Check API rate limits |
| Blank Questions | Verify subject/unit selection |
| Copy Not Working | Check browser clipboard permissions |

## Browser Support

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

## Future Enhancements

- [ ] Database integration for question storage
- [ ] User authentication & progress tracking
- [ ] Export to PDF/Word
- [ ] Offline mode with cached questions
- [ ] Spaced repetition algorithm
- [ ] Performance analytics
- [ ] Multi-language support
- [ ] Mobile app version

## Academic Integrity

This tool is designed for supplementary exam preparation. Students should:
- Use generated questions for practice only
- Understand concepts, not just memorize answers
- Follow institutional academic policies
- Give credit to original course materials

## License

MIT License - Free for personal and educational use

## Support & Issues

For bugs, feature requests, or improvements:
1. Check existing issues in the repository
2. Provide clear reproduction steps
3. Include browser & API details
4. Suggest improvements with examples

## Author

Created for Zoology 4th Semester students at universities using the standard syllabus covering Immunology and Parasitology.

---

**Last Updated**: June 2026  
**Status**: Active & Maintained  
**Version**: 1.0.0
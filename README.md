# AI Resume Analyzer

An AI-powered tool that analyzes resumes for ATS compatibility and job match, 
built with React. Upload a resume (PDF, DOCX, or TXT) and optionally a job 
description to get an instant score, strengths, gaps, and improvement suggestions.

## Features
- Resume upload with PDF and DOCX text extraction (pdf.js, mammoth.js)
- LLM-based analysis: match score, strengths, gaps, actionable suggestions
- Job description matching with keyword overlap scoring
- Local rule-based fallback analyzer if live analysis is unavailable
- Clean, responsive UI built with React and Tailwind CSS

## Tech Stack
- React (hooks: useState, useRef)
- Tailwind CSS
- pdf.js for PDF parsing
- mammoth.js for DOCX parsing
- lucide-react for icons

## How it works
1. User uploads a resume file — text is extracted client-side
2. Resume (+ optional job description) is sent for AI analysis
3. Structured JSON response is parsed and rendered as a score card 
   with strengths, gaps, and suggestions
4. If live analysis fails, a local heuristic scorer (action verbs, 
   quantified achievements, keyword overlap) provides a fallback

## Running locally
\`\`\`
npm install
npm run dev
\`\`\`

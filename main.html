import React, { useState, useEffect, useRef } from 'react';
import { Input } from '@/components/ui/input';
import { Button } from '@/components/ui/button';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';

const paragraphs = [
  "The quick brown fox jumps over the lazy dog. This classic pangram contains every letter of the alphabet.",
  "Programming is the art of telling another human what one wants the computer to do. Code is poetry written for machines.",
  "Learning never exhausts the mind. The more that you read, the more things you will know. The more that you learn, the more places you'll go.",
  "Success is not final, failure is not fatal: it is the courage to continue that counts. Persistence defines true achievement.",
  "In the realm of ideas everything depends on enthusiasm... in the real world all rests on perseverance."
];

const TypingSpeedTester = () => {
  const [currentParagraph, setCurrentParagraph] = useState('');
  const [userInput, setUserInput] = useState('');
  const [startTime, setStartTime] = useState(null);
  const [endTime, setEndTime] = useState(null);
  const [wpm, setWpm] = useState(0);
  const [accuracy, setAccuracy] = useState(0);
  const [mistakes, setMistakes] = useState([]);
  
  const inputRef = useRef(null);

  const startTest = () => {
    const randomParagraph = paragraphs[Math.floor(Math.random() * paragraphs.length)];
    setCurrentParagraph(randomParagraph);
    setUserInput('');
    setStartTime(new Date());
    setEndTime(null);
    setWpm(0);
    setAccuracy(0);
    setMistakes([]);
    inputRef.current.focus();
  };

  const calculateResults = () => {
    const duration = (endTime - startTime) / 60000; // minutes
    const wordCount = currentParagraph.split(' ').length;
    const wordsPerMinute = Math.round(wordCount / duration);
    
    const mistakes = currentParagraph.split('').filter((char, index) => 
      char !== userInput[index]
    );
    
    const accuracyPercentage = Math.round(
      ((currentParagraph.length - mistakes.length) / currentParagraph.length) * 100
    );

    setWpm(wordsPerMinute);
    setAccuracy(accuracyPercentage);
    setMistakes(mistakes);
  };

  const handleInputChange = (e) => {
    const value = e.target.value;
    setUserInput(value);

    if (!startTime) {
      setStartTime(new Date());
    }

    if (value.length === currentParagraph.length) {
      const currentEnd = new Date();
      setEndTime(currentEnd);
      calculateResults();
    }
  };

  useEffect(() => {
    startTest();
  }, []);

  return (
    <Card className="w-full max-w-2xl mx-auto">
      <CardHeader>
        <CardTitle>Typing Speed Tester</CardTitle>
      </CardHeader>
      <CardContent>
        <div className="space-y-4">
          <div className="text-lg bg-gray-100 p-4 rounded">
            {currentParagraph}
          </div>
          
          <Input
            ref={inputRef}
            value={userInput}
            onChange={handleInputChange}
            placeholder="Start typing here..."
            className="w-full p-2 border"
          />
          
          <div className="grid grid-cols-2 gap-4">
            <div>
              <h3 className="font-bold">Words Per Minute</h3>
              <p>{wpm}</p>
            </div>
            <div>
              <h3 className="font-bold">Accuracy</h3>
              <p>{accuracy}%</p>
            </div>
          </div>
          
          {mistakes.length > 0 && (
            <div>
              <h3 className="font-bold">Mistakes</h3>
              <p>{mistakes.join(', ')}</p>
            </div>
          )}
          
          <Button onClick={startTest} className="w-full">
            Restart Test
          </Button>
        </div>
      </CardContent>
    </Card>
  );
};

export default TypingSpeedTester;

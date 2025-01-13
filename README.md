import React from 'react';
import { Card, CardContent } from "@/components/ui/card";
import { Badge } from "@/components/ui/badge";
import { MapPin, Mail, ExternalLink } from 'lucide-react';

const ResumeWebsite = () => {
  const skills = [
    "Product Design & Strategy",
    "Interaction Design",
    "Mobile Application Design",
    "Video/AI User Experience",
    "Hardware Product Design",
    "Design Systems",
    "Public Speaking",
    "Design Education",
    "Inclusive Design",
    "User Research"
  ];

  return (
    <div className="min-h-screen bg-gray-50 py-12 px-4">
      <div className="max-w-4xl mx-auto">
        {/* Header Section */}
        <div className="bg-white rounded-lg shadow-lg p-8 mb-8">
          <div className="flex justify-between items-start">
            <div>
              <h1 className="text-4xl font-bold text-gray-900 mb-2">Kelly Dern</h1>
              <div className="flex items-center text-gray-600 mb-4">
                <MapPin className="w-4 h-4 mr-2" />
                <span>Boulder, Colorado | Remote-Capable</span>
              </div>
              <p className="text-xl text-gray-600">Senior Product Designer</p>
            </div>
          </div>
        </div>

        {/* Main Content Grid */}
        <div className="grid grid-cols-1 lg:grid-cols-3 gap-8">
          {/* Left Column */}
          <div className="lg:col-span-2">
            {/* Experience Section */}
            <Card className="mb-8">
              <CardContent className="pt-6">
                <h2 className="text-2xl font-bold mb-6 text-gray-900">Professional Experience</h2>
                
                <div className="space-y-6">
                  <div>
                    <div className="flex justify-between mb-2">
                      <h3 className="text-lg font-semibold">Senior Product Designer, Video AI</h3>
                      <span className="text-gray-600">Apr 2023 - Present</span>
                    </div>
                    <p className="text-gray-600 mb-2">Google</p>
                    <ul className="list-disc ml-5 text-gray-700 space-y-1">
                      <li>Lead design initiatives for Gemini for Workspace audio/video AI features</li>
                      <li>Recipient of Video Hackathon winner award (May 2023)</li>
                      <li>Drive innovation in video AI user experience and interface design</li>
                    </ul>
                  </div>

                  <div>
                    <div className="flex justify-between mb-2">
                      <h3 className="text-lg font-semibold">Product Designer, Video UX</h3>
                      <span className="text-gray-600">Dec 2018 - Apr 2023</span>
                    </div>
                    <p className="text-gray-600 mb-2">Google</p>
                    <ul className="list-disc ml-5 text-gray-700 space-y-1">
                      <li>Led UX design for Video Monetization & Growth initiatives</li>
                      <li>Spearheaded design systems development for Payments Platform and Workspace</li>
                      <li>Received Google Product Excellence Award (2019)</li>
                    </ul>
                  </div>

                  <div>
                    <div className="flex justify-between mb-2">
                      <h3 className="text-lg font-semibold">Assistant Teaching Professor</h3>
                      <span className="text-gray-600">Apr 2024 - Present</span>
                    </div>
                    <p className="text-gray-600 mb-2">University of Colorado Boulder</p>
                    <ul className="list-disc ml-5 text-gray-700 space-y-1">
                      <li>Graduate faculty for Master of Strategic Communication Design (MSCD) program</li>
                      <li>Teach APRD-5018: Innovative Technologies for Design</li>
                    </ul>
                  </div>
                </div>
              </CardContent>
            </Card>

            {/* Education Section */}
            <Card className="mb-8">
              <CardContent className="pt-6">
                <h2 className="text-2xl font-bold mb-6 text-gray-900">Education</h2>
                <div className="space-y-4">
                  <div>
                    <h3 className="text-lg font-semibold">The London School of Economics and Political Science (LSE)</h3>
                    <p className="text-gray-700">MSc, Media and Communications</p>
                  </div>
                  <div>
                    <h3 className="text-lg font-semibold">Scripps College</h3>
                    <p className="text-gray-700">Bachelor of Arts</p>
                    <p className="text-gray-600">Study abroad: Université Paris-Sorbonne</p>
                  </div>
                </div>
              </CardContent>
            </Card>
          </div>

          {/* Right Column */}
          <div className="space-y-8">
            {/* Skills Section */}
            <Card>
              <CardContent className="pt-6">
                <h2 className="text-2xl font-bold mb-4 text-gray-900">Skills</h2>
                <div className="flex flex-wrap gap-2">
                  {skills.map((skill, index) => (
                    <Badge key={index} variant="secondary" className="text-sm">
                      {skill}
                    </Badge>
                  ))}
                </div>
              </CardContent>
            </Card>

            {/* Achievements Section */}
            <Card>
              <CardContent className="pt-6">
                <h2 className="text-2xl font-bold mb-4 text-gray-900">Achievements</h2>
                <ul className="space-y-2 text-gray-700">
                  <li className="flex items-start">
                    <ExternalLink className="w-4 h-4 mr-2 mt-1 flex-shrink-0" />
                    Google Product Excellence Award (2019)
                  </li>
                  <li className="flex items-start">
                    <ExternalLink className="w-4 h-4 mr-2 mt-1 flex-shrink-0" />
                    Video Hackathon Winner (2023)
                  </li>
                  <li className="flex items-start">
                    <ExternalLink className="w-4 h-4 mr-2 mt-1 flex-shrink-0" />
                    4.6/5 star rating for BOOST Thyroid app
                  </li>
                  <li className="flex items-start">
                    <ExternalLink className="w-4 h-4 mr-2 mt-1 flex-shrink-0" />
                    Regular keynote speaker at international UX conferences
                  </li>
                </ul>
              </CardContent>
            </Card>
          </div>
        </div>
      </div>
    </div>
  );
};

export default ResumeWebsite;

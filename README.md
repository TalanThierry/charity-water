# charity-water
charity water Landing Page
import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

export default function LandingPage() {
  return (
    <div className="min-h-screen bg-white text-gray-900">
      {/* Hero Section */}
      <section className="relative bg-gradient-to-r from-blue-600 to-indigo-600 text-white py-20 px-6 text-center">
        <motion.h1
          initial={{ opacity: 0, y: -30 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
          className="text-4xl md:text-6xl font-bold mb-6"
        >
          Clean Water Changes Everything
        </motion.h1>
        <p className="text-lg md:text-xl mb-8 max-w-2xl mx-auto">
          Together we can bring safe drinking water to communities in need and
          empower the next generation.
        </p>
        <Button size="lg" className="rounded-2xl shadow-lg text-lg px-6 py-3">
          Donate Now
        </Button>
      </section>

      {/* Value Proposition Section */}
      <section className="py-16 px-6 max-w-6xl mx-auto grid md:grid-cols-3 gap-8">
        {[
          {
            title: "Access to Clean Water",
            text: "Every drop transforms health, education, and opportunity.",
            img: "https://via.placeholder.com/400x250",
          },
          {
            title: "Community Empowerment",
            text: "Your support builds lasting infrastructure and hope.",
            img: "https://via.placeholder.com/400x250",
          },
          {
            title: "Next Generation Leaders",
            text: "Inspiring young changemakers to carry the mission forward.",
            img: "https://via.placeholder.com/400x250",
